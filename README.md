# nginx-obs-automatic-low-bitrate-switching

Simple app to automatically switch scenes based on the current bitrate on the nginx stats page.

Uses OBS plugin <a href="https://github.com/Palakis/obs-websocket">obs-websocket</a>.

## Prerequisities

- [Git](http://git-scm.com/)
- [Node.js](http://nodejs.org/) (with NPM)

## Installation

- `git clone <repository-url>`
- Change into the new directory.
- `npm install --production`
- Replace your `nginx.conf` with the one given here.
- Put `stat.xsl` in your nginx folder.

## Config

Edit `config.json` to your own settings.

## How to run

Run the node app by running: `npm start`. Then stream to `rtmp://IPHERE/publish/live`

## Help i can't stream

Make sure the node app is running. It won't allow you to connect to the rtmp without it.

## Help it wont change scenes

It will only change scenes when OBS is set on a scene that's in the config.  
(This is so that it wont change when you're on like your intro scene)
