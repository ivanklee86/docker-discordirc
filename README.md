[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)

This Docker images wraps up the awesome [discord-irc](https://github.com/reactiflux/discord-irc) bot and puts a ribbon on top!

# To run
1. Create a folder for the discord-irc configuration file (e.g. /config).
2. Create a config.json file inside the /config folder (e.g. /config/config.json).  This should be the only file in the directory!
3. Pull the Docker image.
4. Run with the following command, replacing and adding as appropriate.
```
docker run -d -v [PATH_TO_LOCAL_CONFIG]:/app/config docker-discordirc
```

# Build the Image
(This is mainly here for reference.)

To build the container:
```
docker build -t docker-discordirc .
```

To run: (Modify path as appropriate)
```
docker run -it --rm -v /Users/ivanlee/repos/docker-discordirc/config:/app/config docker-discordirc
```