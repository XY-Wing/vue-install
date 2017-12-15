# vue-install
记录下安装vue的过程
- 1、安装brew 
  打开终端运行以下命令：
  ```js
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```
  安装成功后，查看一下brew的版本信息：
  ```js
  brew -v
  ```
- 2、安装node.js 
  在终端中运行以下命令：
  ```js
  brew install nodejs
  ```
  这里由于我已经安装过Xcode，提示：
  ```js
  Error: Xcode alone is not sufficient on Sierra.
  ```
  按照提示，运行以下命令，按照提示安装即可：
  ```js
  xcode-select --install
  ```
- 3、获取nodejs模块安装目录访问权限
  ```js
  sudo chmod -R 777 /usr/local/lib/node_modules/
  ```
- 4、安装 淘宝镜像 （npm）：安装完成后，所有用到npm的地方都可以替换为cnpm，速度一级快。
  ```js
  npm install -g cnpm --registry=https://registry.npm.taobao.org
  ```
- 5、安装webpack
  ```js
  cnpm install webpack -g
  ```
- 6、安装vue脚手架
  ```js
  npm install vue-cli -g
  ```
- 7、在硬盘上找一个文件夹放工程用的，在终端中进入该目录

- 8、根据模板创建项目，完成后会要求输入一些初始项
  ```js
  vue init webpack-simple 工程名字<工程名字不能用中文和大写字母>
  ```
- 9、进入创建的工程目录

- 10、安装项目依赖
  ```js
  cnpm install
  ```
  
- 11、安装 vue 路由模块vue-router和网络请求模块vue-resource
  ```js
  cnpm install vue-router vue-resource --save
  ```
- 12、启动项目	
  ```js
  npm run dev
  ```
完成后便可用编辑器打开项目了。

  
 
