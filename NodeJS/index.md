# Nodejs

## 快捷安装

### Ubuntu

```bash
sudo apt-get update
sudo apt-get install -y python-software-properties software-properties-common
sudo add-apt-repository ppa:chris-lea/node.js

sudo apt-get update
sudo apt-get install nodejs
sudo apt install nodejs-legacy
sudo apt install npm

# 继续安装node包管理，安装方法在下面
```

### macOS

```bash
curl "https://nodejs.org/dist/latest/node-${VERSION:-$(wget -qO- https://nodejs.org/dist/latest/ | sed -nE 's|.*>node-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/node-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/node-latest.pkg" -target "/"

# or

brew install node

# or

port install nodejs<major version>  # port install nodejs7
```

## 下载安装

[下载地址](https://nodejs.org/zh-cn/download/)

## 通过包管理器方式安装

- [安装地址](https://nodejs.org/zh-cn/download/package-manager/)

## 其他安装方法

- [在 Linux 上，通过二进制文件安装 Node.js](https://github.com/nodejs/help/wiki/Installation)
- [在支持的平台上，使用源代码构建 Node.js](https://github.com/nodejs/node/blob/master/BUILDING.md#building-nodejs-on-supported-platforms)

## 安装包管理器

选择nvm或n，作为Nodejs包管理工具

### nvm

- [nvm安装或升级](https://github.com/nvm-sh/nvm#installation-and-update)

### n

```bash
sudo npm install n -g
sudo n stable #安装最新的nodejs（stable版本）
sudo node -v
```

## NPM

```bash
# 更新npm的包镜像源，方便快速下载
sudo npm config set registry https://registry.npm.taobao.org

# 升级npm
npm install -g npm 
```
