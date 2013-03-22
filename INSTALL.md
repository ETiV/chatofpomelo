INSTALL
------

After cloned, you may run `sh npm-install.sh` command at the root of repository directory to install the dependent packages.

Configuration
------

To run this demo in public, config file is need to be modified.

First of all, make clear your server's ip address. For example, `192.168.1.140`.

Open `game-server/config/servers.json` with your editor. You should see several `"clientHost":"127.0.0.1"`.

Now let's **ONLY** change this `clientHost` key's value to your server's ip address, like this: `"clientHost":"192.168.1.140"`.

Change all the others `clientHost` key's value. Then save this configuration file.

Run
-----

If you have installed `pomelo` globally, you can just run `pomelo start` at `game-server`.
At the `web-server` directory, type `node app.js` to run.

Still you can see `Please log on http://127.0.0.1:3001/index.html`, but the server is working in public area(at lease LAN accessable).
So, open your browser, open the link by your ip address. For example: `http://192.168.1.140:3001`.

Share this link to other people. They can talk at your own chat server now.