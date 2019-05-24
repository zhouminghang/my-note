使用 **Chrome** 浏览器开发 **Vue** 项目的时候，控制台提示：


> Download the Vue Devtools extension for a better development experience:
https://github.com/vuejs/vue-devtools


![QQ截图20190522161528.png](https://upload-images.jianshu.io/upload_images/5726812-fd205ee508d60efd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


这个工具可以查看组件状态，`加快开发效率`。

如果你能 `翻墙`，可以直接在谷歌的应用商店安装`vue-devtools`, 没有梯子的可以继续往下看😀👇：

[我也刚玩，不知道是啥，去load一把，传送门====》https://github.com/vuejs/vue-devtools](https://github.com/vuejs/vue-devtools)

### 1. 克隆、下载随意： 

![QQ截图20190522162000.png](https://upload-images.jianshu.io/upload_images/5726812-9c8f62d00e9b8406.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2. 本地解压：
![QQ截图20190522162333.png](https://upload-images.jianshu.io/upload_images/5726812-ded6683ff74d6a99.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 3. 进入解压后的目录(我的解压后的文件夹名自己修改过)，然后 `npm install` 安装依赖：
![QQ截图20190522162356.png](https://upload-images.jianshu.io/upload_images/5726812-16a42a624e7770ba.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

如下代表成功：
```
Microsoft Windows [版本 10.0.17763.437]
(c) 2018 Microsoft Corporation。保留所有权利。

I:\浏览器下载\Chrome_Download\vue-devtools>npm install
npm WARN deprecated joi@13.7.0: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm WARN deprecated hoek@5.0.4: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm WARN deprecated hoek@6.1.3: This module has moved and is now available at @hapi/hoek. Please update your dependencies as this version is no longer maintained an may contain bugs and security issues.

> core-js@2.6.8 postinstall I:\浏览器下载\Chrome_Download\vue-devtools\node_modules\core-js
> node -e "try { require('./scripts/postinstall'); } catch (e) { /* empty */ }"

Thank you for using core-js ( https://github.com/zloirock/core-js )!

Please consider supporting of core-js on Open Collective or Patreon:
> https://opencollective.com/core-js
> https://www.patreon.com/zloirock

Also, the author of core-js ( https://github.com/zloirock ) is looking for a good job -)


> cypress@3.3.0 postinstall I:\浏览器下载\Chrome_Download\vue-devtools\node_modules\cypress
> node index.js --exec install

Installing Cypress (version: 3.3.0)

 √  Downloaded Cypress
 √  Unzipped Cypress
 √  Finished Installation C:\Users\ZMH\AppData\Local\Cypress\Cache\3.3.0

You can now open Cypress by running: node_modules\.bin\cypress open

https://on.cypress.io/installing-cypress


> webpack-cli@3.3.2 postinstall I:\浏览器下载\Chrome_Download\vue-devtools\node_modules\webpack-cli
> node ./bin/opencollective.js



                            Thanks for using Webpack!
                 Please consider donating to our Open Collective
                        to help us maintain this package.



                 Donate: https://opencollective.com/webpack/donate


npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@1.2.9 (node_modules\fsevents):
npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.2.9: wanted {"os":"darwin","arch":"any"} (current: {"os":"win32","arch":"x64"})

added 1003 packages in 550.53s
```

### 4. 安装完依赖后，执行 `npm run build` 构建工具。 
![QQ截图20190522163527.png](https://upload-images.jianshu.io/upload_images/5726812-729c94b5835a4611.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

成功如下：
```
I:\浏览器下载\Chrome_Download\vue-devtools>npm run build

> vue-devtools@5.1.0 build I:\浏览器下载\Chrome_Download\vue-devtools
> cd shells/chrome && cross-env NODE_ENV=production webpack --progress --hide-modules

 98% after emitting SizeLimitsPlugin

 DONE  Compiled successfully in 23671ms                                                                         16:35:58

Hash: d8f5410543cda1de0f16
Version: webpack 4.32.1
Time: 23671ms
Built at: 2019-05-22 16:35:58
                 Asset      Size  Chunks                    Chunk Names
            backend.js   391 KiB       0  [emitted]  [big]  backend
         background.js  2.59 KiB       1  [emitted]         background
           detector.js  4.31 KiB       2  [emitted]         detector
devtools-background.js  2.22 KiB       4  [emitted]         devtools-background
           devtools.js  1.08 MiB       3  [emitted]  [big]  devtools
               hook.js  28.3 KiB       5  [emitted]         hook
              proxy.js   1.3 KiB       6  [emitted]         proxy
Entrypoint hook = hook.js
Entrypoint devtools [big] = devtools.js
Entrypoint background = background.js
Entrypoint devtools-background = devtools-background.js
Entrypoint backend [big] = backend.js
Entrypoint proxy = proxy.js
Entrypoint detector = detector.js
```
### 5. 打开Chrome `扩展程序`，`开启` 开发者模式，`加载已解压的扩展程序`:
![QQ截图20190522163928.png](https://upload-images.jianshu.io/upload_images/5726812-5a56b8dcc044d347.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

选择`shells`目录下的`chrome`文件夹:
![QQ截图20190522164057.png](https://upload-images.jianshu.io/upload_images/5726812-e21ebb9000d82378.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

`启用`拓展程序:
![QQ截图20190522164248.png](https://upload-images.jianshu.io/upload_images/5726812-08e907e82c6f2711.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



![QQ截图20190522164337.png](https://upload-images.jianshu.io/upload_images/5726812-6a97c108bfe72fa6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 6. 重启Chrome，打开控制台，点击Vue，查看即可。

![QQ截图20190522165240.png](https://upload-images.jianshu.io/upload_images/5726812-4f241b38b088a4c4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 7. 关于 npm install失败、npm run build失败。
本机环境：
* node `v8.10+`
* npm 用的`taobao`源

网上有的小伙伴`npm install` 或者 `npm run build`失败。

* 建议切换淘宝镜像，或者使用`cnpm`、`yarn`
* `nrm`可以方便切换npm源。
* `node 版本太低`，建议8.10+
* `nvm`可以方便切换node版本。


网上参考地址：

* https://www.cnblogs.com/yuqing6/p/7440549.html

* https://segmentfault.com/a/1190000009682735?utm_source=tag-newest