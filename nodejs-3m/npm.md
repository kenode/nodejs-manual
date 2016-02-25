# 安装 `Node.js` 和 `npm` 包管理器

`npm` 是 Node Package Manager 的缩写，即 `Node.js` 的包管理器。

## 安装 `Node.js`

查看所有远程版本：
```bash
$ nvm ls-remote
```

查看本地安装版本：
```bash
$ nvm ls
```

安装 `4.x` 稳定版
```bash
$ nvm install 4
```

安装 `5.x` 开发版
```bash
$ nvm install 5
```

切换当前 `Node.js` 版本
```bash
$ nvm use 4  # 切换到 4.x 版本
$ nvm use 5  # 切换到 5.x 版本
```

设置系统 `Node.js` 版本
```bash
$ nvm alias default 4  # 设置 4.x 为系统版本
$ nvm alias default 5  # 设置 5.x 为系统版本
```

## 安装 `npm`

`npm` 随 `Node.js` 一起安装

安装指定版本
```bash
$ npm i -g npm@2  # 安装 2.x 版本
$ npm i -g npm@3  # 安装 3.x 版本
```
