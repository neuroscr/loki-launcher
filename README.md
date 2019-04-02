
# Requirements

- [nodejs](https://nodejs.org/en/) 8.x or later
- [lokid](https://github.com/loki-project/loki)
- [lokinet](https://github.com/loki-project/loki-network)
- [httpserver (storage server)](https://github.com/loki-project/loki-storage-server)
- Linux (though macos does works and Windows kind of works)

You can download the loki binaries (faster) from each above page's release section
or
You can build from source, you can use the [init.sh](init.sh) script to pull the latest source.

# How to run

edit the config [launcher.ini](launcher.ini) and check over the settings, [Check our wiki](https://github.com/loki-project/loki-launcher/wiki/Launcher.ini-configuration-documentation) for details on options.

`node index.js`

If interactive is true, then this will provide an interactive console with lokid with lokinet running in the background
`exit` will quit both.

If interactive is fale, then it will validate the environment, let you know of any problems and potentially start the servers into the background (it will be safe to disconnect from the terminal and they should continue running).

# Popular ways to install nodejs

Ubuntu node installation:

`curl -sL https://deb.nodesource.com/setup_10.x | sudo bash -`

then

`sudo apt-get install -y nodejs`
