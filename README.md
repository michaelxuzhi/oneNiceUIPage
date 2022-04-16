# 如何将项目run起来，步骤：

##### 参考1： [electron的安装教程](https://blog.csdn.net/michaelxuzhi___/article/details/109138552?spm=1001.2014.3001.5501)
##### 参考2：[electron打包失败解决](https://blog.csdn.net/michaelxuzhi___/article/details/106568543?spm=1001.2014.3001.5501)

#### · 步骤一：因为要用到electron，国内下载的速度较慢，所以用国内镜像成功率较高，推荐使用：淘宝镜像，切换方式：
```js
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

#### · 步骤二：依赖的安装：因为我们切换了包管理源，所以`cnpm install` 代替了原本的`npm install` ，执行`cnpm i`
#### · 步骤三：（网页版）等待依赖完成，执行 `npm run serve` 项目跑起来
#### · 步骤三：（客户端版）等待依赖完成，执行 `npm run electron:serve` 项目跑起来
