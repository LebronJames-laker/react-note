# MongoDB的安装

- 首先从官网下载MongoDB https://www.mongodb.com/download-center/enterprise  

  ![1587168130112](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587168130112.png)

- 下载完成之后，开始安装配置

  双击打开文件进行安装，在安装过程中，可以通过点击 "Custom(自定义)" 按钮来设置你的安装目录。

  ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327110956254-767522594.png)

  这里我选择安装在E:\MongoDB这个目录下（安装目录会影响我们后面的配置）。

  ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327111030712-1940620224.png)

  这里选择直接next：

  ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327111202101-1153181920.png)

  这里安装 **"Install MongoDB Compass"** 不勾选，否则可能要很长时间都一直在执行安装，MongoDB Compass是一个图形界面管理工具，这里不安装也是没有问题的，可以自己去下载一个图形界面管理工具，比如[Robo3T](https://robomongo.org/)。

  ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327111309421-1373386005.png)

  之后稍微等待一会就安装好了。

   **配置数据库文件所存放的位置**

  MongoDB的安装过程是很简单的，但是配置就比较麻烦了，可能会遇到各种各样的问题，需要你有足够的耐心和仔细。

  首先要在MongoDB的data文件夹里新建一个db文件夹和一个log文件夹：

  ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327111744600-236215096.png)

  然后在log文件夹下新建一个mongo.log：

   ![img](https://img2018.cnblogs.com/blog/1450803/201903/1450803-20190327111924389-669177821.png)

- 启动MongoDB服务

  **首先可以配置一下全局变量**

  ![1587168382067](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587168382067.png)

  进入cmd命令窗口，输入

  `mongod --dbpath D:\Program Files\MongoDB\Server\4.2\data`

![1587168433732](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587168433732.png)

**配置成功**

![1587168703088](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587168703088.png)

# React安装Node

- 官网下载node

![1587171921373](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587171921373.png)

![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190603182606186-651619511.png)

　　点击下一步，勾选接受许可

　　![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190603182649337-972452582.png)

　　点击下一步，选择安装目录，我的安装目录是D:\xiaofeng\nodejs\

　　![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190603182802499-1515714087.png)

　　点击下一步，个人设置选择可以选择默认的

　　![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190603182859910-984777052.png)

　　然后开始安装

　　![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190603182916301-828859879.png)

　　![img](https://img2018.cnblogs.com/blog/1033563/201906/1033563-20190604094641778-14970732.png)

　　安装完成之后，我们可以检验一下是否安装完成，按win+r，输入cmd打开命令行，输入node -v查看node的版本，输入where node查看node命令的路径



# React安装全局脚手架

```java
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

![1587171819820](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587171819820.png)

安装完成之后，输入`cnpm -v`,出现如下，表示安装成功

![1587171864874](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587171864874.png)

安装好淘宝镜像之后，开始全局安装脚手架

```java
cnpm install -g create-react-app
```

![1587172263364](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587172263364.png)

**安装成功！！！**



利用脚手架创建react项目

```java
create-react-app react-admin-client
```

![1587173193570](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587173193570.png)

输入如下命令即可看到效果！！

```
npm start
```

![1587173403603](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587173403603.png)

输入如下命令进行打包！

```java
npm run build
```

全局下载服务（将来是要部署到这个上面的）

```java
npm install -g serve
```

输入如下命令，将项目部署到本地服务器上

```java
serve build
```

![1587174045159](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587174045159.png)

结果如下

![1587174081531](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587174081531.png)

[**git的安装教程**]: https://blog.csdn.net/sishen47k/article/details/80211002?depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-1&amp;utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-1

提交项目到github

![1587176033172](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587176033172.png)

 ![img](https://img-blog.csdn.net/20180117221426174?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbTBfMzgwMjIwMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast) 

```java
$ git pull origin master --allow-unrelated-histories //输入此段指令
```

> 在本地中创建一个项目所在的文件夹
>
> 2、npm -g create-react-app
>
> 3、在此文件夹下 create-react-app react-demo (项目名)
>
> 4、cd react-demo
>
> 5、npm start（等待一会浏览器自动开启）
>
> 6、开始噼里啪啦写你需要的代码
>
> 7、（重点）在package.json配置文件中加一句：　“homepage”: “./” （为下面打包做准备，如果不加这句话，那么在预览时开启的页面空白，原因路径不对）
>
> 8、npm run build（打包）
>
> 9、在你的GitHub上新建个仓库，把地址复制下来备用
>
> 10、项目所在文件夹下git init
>
> 11、git add . （点的意思是所有文件，把所有文件添加上去）
>
> 12、git commit -m "xxxxxxxxxx"（提交信息）
>
> 13、git remote add origin https://github.com/xxx/xxx（刚才你在GitHub上保存的地址）
>
> 14、git pull origin master（上传之前先拉一下，第一次不拉也行，但是之后提交最好想成这个习惯）
>
> 15、git push -u origin master（把你的代码提到GitHub上）
>
> 16、此时，在GitHub对应的仓库上，就可以看到刚才提交的代码了。
>
> 　　接着，点击“setting”；
>
> 　　找到GitHub Pages，source中点击下面按钮切换到master branch，点击save；
>
> 　　就可以看到一个链接了，点击链接，发现出现的是你项目中的README.md；
>
> 　　在链接后面加上  /build/#  回车后，即可看到预览效果。 
>
> 之后的修改代码后，重新npm run build ，重复11~15步骤即可。

**git push的时候出现问题**

```java
$ git push origin master
To https://github.com/LebronJames-laker/mine-react.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/LebronJames-laker/mine-react.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.


```

**git**

![1587390249346](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587390249346.png)

```java
$ git push origin dev //把代码提交到远程的dev分支中
fatal: HttpRequestException encountered.
   ▒▒▒▒▒▒▒▒ʱ▒▒▒▒
Username for 'https://github.com': LebronJames-laker
To https://github.com/LebronJames-laker/mine-react.git
 ! [rejected]        dev -> dev (non-fast-forward)
error: failed to push some refs to 'https://github.com/LebronJames-laker/mine-react.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
    //此时出现错误
原因是：
未能将一些参考资料推入库中，更新被拒绝，因为当前分支的提示在后面！
这是由于github的版本库没有pull到本地，这样就产生了远程repository和本地的repository的版本冲突。
```

解决：

![1587365927483](C:\Users\xys\Desktop\1587365927483.png)

![1587390276139](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587390276139.png)

重新commit然后pull拉取一下，最后push到远程

```java
 * branch            master     -> FETCH_HEAD
fatal: refusing to merge unrelated histories //出现这个问题

```

![1587373011500](C:\Users\xys\AppData\Roaming\Typora\typora-user-images\1587373011500.png)

![1587390308973](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587390308973.png)

此时head分支从origin/dev中游离出去了

输入如下命令即可解决：

![1587219122967](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587219122967.png)

结果如下：

![1587219178917](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587219178917.png)

```java
$ git checkout -b dev
Switched to a new branch 'dev'	//创建一个新的分支
```

查看自己的分支

![1587221060988](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587221060988.png)

删除自己本地的分支

![1587221272838](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587221272838.png)

```java
git checkout -b dev origin/dev //表示在本地创建并选中dev分支，那么这个dev分支是复制远程的dev分支
```



![1587221393052](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587221393052.png)

**此时可能会出现，删不了的情况，因为此时你正在使用这个分支，此时只需要切换到别的分支即可**

# 安装antd的时候出现问题

![1587262787392](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587262787392.png)

![1587262771283](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587262771283.png)

以管理员的身份运行powershell，并输入` set-ExecutionPolicy RemoteSigned `,更改脚本执行的权限

# 开始引入antd

完成上面的更改权限的操作之后，开始如下操作

- 输入命令`yarn add antd` 安装antd库

- 更改app.js文件

  ```js
  import React from 'react';
  import { Button,message} from 'antd'
  import 'antd/dist/antd.css' //此时只是初级版，引入antd.css样式文件，之后会按需导入
  //自定义一个App组件
  export default class App extends React.Component{
      //此时这里用箭头函数。会保证下面this的准确性
      handleClick=()=>{
          message.success("成功啦，我的React项目搭起来啦")
      }
      render(){
          return <Button type="primary" onClick={this.handleClick}>点击我</Button>
      }
  
  }
  ```

- 此时的效果图如下

  ![1587267022873](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587267022873.png)

- 输入如下命令，` yarn add react-app-rewired customize-cra `,准备按需导入

- 修改package.json文件的内容 加号代表需要加入的，减号代表需要删除原先的

  ```json
  /* package.json */
  "scripts": {
  -   "start": "react-scripts start",
  +   "start": "react-app-rewired start",
  -   "build": "react-scripts build",
  +   "build": "react-app-rewired build",
  -   "test": "react-scripts test",
  +   "test": "react-app-rewired test",
  }
  ```

-  然后在项目根目录创建一个 `config-overrides.js` 用于修改默认配置。 

  这个文件的最终内容如下：

  ```js
  + const { override, fixBabelImports } = require('customize-cra');
  
  - module.exports = function override(config, env) {
  -   // do stuff with the webpack config...
  -   return config;
  - };
  + module.exports = override(
  +   fixBabelImports('import', {
  +     libraryName: 'antd',
  +     libraryDirectory: 'es',
  +     style: 'css',
  +   }),
  + );
  ```

- 但是在修改成最终版之前需要下载安装一个插件

  ```js
  yarn add babel-plugin-import
  ```

-  然后移除前面全量添加的 `@import '~antd/dist/antd.css';` 样式代码，并且按下面的格式引入模块。 

  **此时出现了一个巨坑的地方，如下图所示**

![1587289721256](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587289721256.png)

项目跑不起来！！！非常值得注意一点，官网有一段话这么说的！！

![1587289769691](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587289769691.png)

在项目的根目录下创建config-overrides.js文件，注意是根目录，我在这里错误的放在了src文件下，导致项目一直跑不起来，如图：放在这个位置即可

![1587289857629](C:\Users\科比布莱恩特\AppData\Roaming\Typora\typora-user-images\1587289857629.png)

内容如下：

```js
const { override, fixBabelImports } = require('customize-cra');

// - module.exports = function override(config, env) {
// -   // do stuff with the webpack config...
// -   return config;
// - };
module.exports = override(
   fixBabelImports('import', {//这个import代表的是"babel-plugin-import": "^1.13.0" 这个我们需要用到的插件的标识，因为babel的插件都是babel-plugin开头，所以看后缀就可以区分各个插件
     libraryName: 'antd',
     libraryDirectory: 'es',
     style: 'css',
   }),
 );
```

