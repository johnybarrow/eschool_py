# Eschool

Best python library to work with Eschool electronic diary (https://eschool.center)

## Getting Started

Logging in for the first time:

```python
from eschool_lib import EschoolClient


client = EschoolClient.login('your_username', 'your_password')
# you can also write Eschool.login('your_username') and you will be prompted for your password
```


Getting marks, homeworks and chats:
```python
client.marks()
client.homeworks()  # Real homeworks
client.get_homeworks() # Flash homeworks
client.get_homeworks((1, 10, 2019))  # Homework for the date
client.get_homeworks((1, 10, 2019), (10, 10, 2019))  # Homework since ... to ... (flash)  
```

### Installing

For Linux:
```bash
sudo pip3 install eschool_lib
```

For Windows:
```bash
pip install eschool_lib
```
