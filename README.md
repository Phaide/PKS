# Port-knocking
A port-knocking utility. 

## Issue
Opening a server publicly to the Internet implies major risks.<br />
Along with different ways of securing its access, such as RSA keys for SSH connections, I learned about a server-side system allowing outside connections "on-demand" using a knocking system, that will open a port once a specific sequence of packets is received.<br />

A bunch of articles have already been written on the subject, such as this paper, which is pretty interesting and accurate :<br />
https://www.sans.org/reading-room/whitepapers/sysadmin/port-knocking-basics-1634<br />

It covers the main problem with port-knocking systems : static port-knocking.<br />

## Solution
This script, written in Python 3, is an attempt to solve this issue by dynamically defining new ports sequences.<br />
However, it is not flawless ; therefore it is not advised in its current state to use it in a production environment. 
It's rather an experimental feature to build upon.<br />

## Future work
As of March 2020, the main future work is to proofread the code, debug and test.<br />
I'm mainly working on simplifying the code currently.<br />
Also, Windows support for the daemon would be appreciated.<br />
New features requests are welcome.<br />

## Usage
Use the following command (Python 3) to list the options
```
python port_knocking_utility.py -h
```

## Contributing
If you want to contribute, please fork this repo and/or send pull requests. Thank you.<br />

## Supporting
If you want to support me, you can send some kind messages via my website (https://phaide.net/contact)<br />

And perhaps, consider making a donation<br />

    BTC: 178oEM3sUYtHVYVt2jbHv4HNjy2nfu1iiT
    ETH: 0x4f3290b22012f0d01900a87e4475c01a7f95ee93

With love,<br />
Phaide.
