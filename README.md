
You will need some other Lua modules too, which can be (and should be) installed through the Lua package manager LuaRocks.

**Installation**
```bash
# Tested on Ubuntu 14.04, Ubuntu 15.04, Debian 7, Linux Mint 17.2

$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install libreadline-dev libssl-dev lua5.2 liblua5.2-dev git make unzip redis-server curl libcurl4-gnutls-dev

# We are going now to install LuaRocks and the required Lua modules

$ wget http://luarocks.org/releases/luarocks-2.2.2.tar.gz
$ tar zxpf luarocks-2.2.2.tar.gz
$ cd luarocks-2.2.2
$ ./configure; sudo make bootstrap
$ sudo luarocks install luasocket
$ sudo luarocks install luasec
$ sudo luarocks install redis-lua
$ sudo luarocks install lua-term
$ sudo luarocks install serpent
$ sudo luarocks install dkjson
$ sudo luarocks install lanes
$ sudo luarocks install Lua-cURL
$ cd ..

# Clone the repository and give the launch script permissions to be executed

$ git clone https://github.com/shahabdark/GroupButler.git
$ cd GroupButler
$ sudo chmod 777 launch.sh
```

