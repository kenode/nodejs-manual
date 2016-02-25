# 安装 `nvm` 版本管理器

`nvm` 是 Node Version Manager 的缩写，即 `Node.js` 的版本管理器。

仓库地址：[https://github.com/creationix/nvm](https://github.com/creationix/nvm)

## 安装`nvm`

**Curl** 方式：
```bash
$ cd ~ && curl -o- https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

**Wget** 方式：
```bash
$ cd ~ && wget -qO- https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

## 更新 `nvm`

```bash
$ cd "$NVM_DIR" && git pull origin master && git checkout `git describe --abbrev=0 --tags`
```