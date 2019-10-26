# Nodejs

## Quick installation

### Ubuntu

```bash
sudo apt-get update
sudo apt-get install -y python-software-properties software-properties-common
sudo add-apt-repository ppa:chris-lea/node.js

sudo apt-get update
sudo apt-get install nodejs
sudo apt install nodejs-legacy
sudo apt install npm

# or

nvm install latest # Install nvm first, the installation method is below
```

### macOS

```bash
curl "https://nodejs.org/dist/latest/node-${VERSION:-$(wget -qO- https://nodejs.org/dist/latest/ | sed -nE 's|.*>node-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/node-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/node-latest.pkg" -target "/"

# or

brew install node

# or

port install nodejs<major version>  # port install nodejs7
```

## Download and install

[Download link](https://nodejs.org/zh-cn/download/)

## Installed by package manager

- [Installation address](https://nodejs.org/zh-cn/download/package-manager/)

## Other installation methods

- [Installing Node.js via binary archive on Linux](https://github.com/nodejs/help/wiki/Installation)
- [Building Node.js from source on supported platforms](https://github.com/nodejs/node/blob/master/BUILDING.md#building-nodejs-on-supported-platforms)

## Installation package manager

Choose nvm or n as the Nodejs package management tool

### nvm

- [Nvm installation or upgrade](https://github.com/nvm-sh/nvm#installation-and-update)

### n

```bash
sudo npm install n -g
sudo n stable #Install the latest nodejs (stable version)
sudo node -v
```

## NPM settings

```bash
# Update the npm package image source for quick download
sudo npm config set registry https://registry.npm.taobao.org
sudo npm config list
```
