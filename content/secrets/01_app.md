---
draft: false
weight: 1990
---
```python
#!/usr/bin/env python
"""Dummy project"""
from __future__ import print_function

import socket
import os

import flask


APP = flask.Flask(__name__)
PATH = os.getenv("COUNTER_PATH")


def get_counter():
    """Get the counter from the local storage."""
    try:
        return int(open(PATH, "r").read())
    except Exception as exc:
        print("Exception :", exc)
        return 0

def inc_counter():
    """Increment the local storage counter."""
    c = get_counter()
    with open(PATH, "w") as fd:
        fd.write(str(c + 1))

@APP.route("/")
def index():
    """Return index."""
    inc_counter()
    return "[{}] Hello Mambu Labs {}".format(
        get_counter(),
        str(socket.gethostname())
    )


if __name__ == "__main__":
    APP.run(host="0.0.0.0", port=8080, debug=True)
```
