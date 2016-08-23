#  安装 nrm

Node.js 安装好之后，其自带 npm 包管理器；由于 npm 仓库位于国外，我们需要切换到国内的镜像站点。

nrm 是一个 npm 源管理器，允许你快速地在如下 NPM 源间切换。

### 安装

```bash
$ npm i -g nrm
```

### 使用

列出所有的源
```bash
$ nrm ls

* npm ---- https://registry.npmjs.org/
  cnpm --- http://r.cnpmjs.org/
  taobao - http://registry.npm.taobao.org/
  edunpm - http://registry.enpmjs.org/
  eu ----- http://registry.npmjs.eu/
  au ----- http://registry.npmjs.org.au/
  sl ----- http://npm.strongloop.com/
  nj ----- https://registry.nodejitsu.com/
  pt ----- http://registry.npmjs.pt/
```

测试所有源速度
```bash
$ nrm test

* npm ---- 935ms
  cnpm --- 209ms
  taobao - 176ms
  edunpm - 341ms
  eu ----- Fetch Error
  au ----- Fetch Error
  sl ----- 825ms
  nj ----- 1714ms
  pt ----- Fetch Error
```

测试指定源速度
```bash
$ nrm test taobao

  taobao - 89ms
```

打开指定源官网
```bash
$ nrm home taobao
```

切换到指定源
```bash
$ nrm use taobao

   Registry has been set to: http://registry.npm.taobao.org/
```

查看当前源
```bash
$ nrm current
taobao
```

添加自定义源，适合自己的私有源
```bash
$ nrm add kenode http://registry.npm.kenode.org/ http://npm.kenode.org

    add registry kenode success
```

删除源
```bash
$ del kenode
```