# Star Libary

This is the Star Libary, it is written in many languages such as

* [Lua](lua.org)

* [Python](python.org)

* [JavaScript (Node.js)](nodejs.org)

# Installation

If you downloaded the full version of [Star](star-corp.hopto.org)  the libary allready comes with it

Else we reccomend you download the full version of [Star](star-corp.hopto.org) 

Anyway, if you would like to download it seperatley follow theese instructions

First, download the [setup file](https://raw.githubusercontent.com/Star-Corporation/Star-Utils/master/star-lib-setup.sh) then follow theese steps:

1) Open a terminal window (not `cmd.exe`) (must support bash and shell scripts)

2) Use the `cd` command to cd into the folder where the setup file is, e.g

```sh
cd Downloads
```

3) Depending on what language of the libary you want to install do the following:

If you want to install the libary in all supported languages (Recommended) type:

```sh
sh star-lib-setup.sh all
```

If you want to install the libary in Python type:

```sh
sh star-lib-setup.sh python
```

If you want to install the libary in Lua type:

```sh
sh star-lib-setup.sh lua
```

Else, if you want to install the JavaScript (Node.js) version type:

```sh
sh star-lib-setup.sh node
```

If you just type:

```sh
sh star-lib-setup.sh
```

You will get a error made by the setup script

4) Star is now installed, please see the usage section to see how to use it

# Usage

Its fairly simple to use the Star Libary

Lua:

```lua
local uname = "USERNAME_STAR_IS_INSTALLED_ON"
local Star = require("/home/"..uname.."/Star/StarLibLua")
local PC = Star.PC
local Server = Star.Server
local Client = Star.Client
local Network = Star.Network

Star.Loaded(function()
print('Ready!')
end)
```

JavaScript:

```javascript
const uname = "USERNAME_STAR_IS_INSTALLED_ON"
const Star = require('/home/' + uname + '/Star/StarLibJS.js');
const PC = Star.PC;
const Client = Star.Client;
const Server = Star.Server;
const Network = Star.Network;

Star.Loaded(function(){
console.log('Ready!');
});
```

Python:

```python
import sys

uname = "USERNAME_STAR_IS_INSTALLED_ON"

sys.path.append('/home/' + str(uname) + '/Star')

import StarLibPython as Star

Network = Star.Network
Server = Star.Server
Client = Star.Client
Pc = Star.Pc

Star.Loaded(
def():
      print('Ready!')
)
```
