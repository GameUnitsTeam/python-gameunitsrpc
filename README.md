AuthServiceProxy is an improved version of python-jsonrpc.

![Gameunits](http://i.imgur.com/Cokp8iC.png)

It includes the following generic improvements:

- HTTP connections persist for the life of the AuthServiceProxy object
- sends protocol 'version', per JSON-RPC 1.1
- sends proper, incrementing 'id'
- uses standard Python json lib

It also includes the following gameunits-specific details:

- sends Basic HTTP authentication headers
- parses all JSON numbers that look like floats as Decimal

Installation:

- change the first line of setup.py to point to the directory of your installation of python 2.*
- run setup.py

Note: This will only install gamerscoinrpc. If you also want to install jsonrpc to preserve 
backwards compatibility, you have to replace 'gamerscoinrpc' with 'jsonrpc' in setup.py and run it again.
