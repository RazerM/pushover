A simple Python3.3 client for http://pushover.net/ API based off of https://github.com/pix0r/pushover by pix0r.

Install:

    pip install https://github.com/Wyattjoh/pushover

Sample Python3 Usage:

```python
from pushover import Pushover

po = Pushover("My App Token")
po.set_user("My User Token")

msg = po.msg("Hello, World!")

msg.set("title", "Best title ever!!!")

po.send(msg)
```

Sample Shell Usage:

```bash
./pushover "Hello, World!" --token="My App Token" --user="My User Token"
```
