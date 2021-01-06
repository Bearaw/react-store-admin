
这个项目基于`react + antdesign + react-router + redux + axios + mock + AMap + echarts`等技术栈完成。

## 项目介绍

注意：现在项目并没有全部完成，部分功能待开发

项目运行地址：https://chengllnice.github.io/react-store-admin/

项目运行

```javascript
git clone https://github.com/chengllNice/react-store-admin.git

cd react-store-admin

cnpm i

npm start

```



### 首先进入登录界面

`默认可以登录的账号`

账号：root，密码：123456

账号：bussiness，密码：123456


### 登录之后进入首页

右上角可以进入主题皮肤的切换，现在支持4中皮肤


## 项目目录简介

主要目录介绍：

    config                  ----webpack配置目录
    public
    scripts                 ----命令
    src                     ----源码目录
        ----assets          ----静态文件目录
            ----css         ----全局css目录
            ----images      ----图片
        ----auth            ----权限配置目录（暂时没做权限配置）
        ----components      ----公用组件
        ----config          ----公用配置（不是webpack的配置，而是项目的全局配置）
        ----mock            ----mock数据
        ----redux           ----redux目录
        ----routers         ----路由目录
        ----servers         ----接口请求
        ----utils           ----工具方法
        ----views           ----各模块代码主目录
        ----index.js        ----项目入口文件
        

###   src--config目录说明

name:配置项目名称

leftNavdefaultOpenAll: 是否默认展开所有侧导航一级菜单。  true展开  false不展开。如果配置为false,会展开当前路由所在的一级菜单，其他全部默认关闭。

CollapseModel：侧导航切换的模式。true为手风琴模式

collapsedDefaultOpen：默认是否展开侧导航。true展开  false收起

mock：是否使用mock数据。如果是生产环境此项配置不生效(暂无真实接口支持，只能用mock数据接口)

```javascript

module.exports = {
  name: 'X-Admin',
  leftNavdefaultOpenAll: false,
  CollapseModel: true,
  collapsedDefaultOpen: false,
  mock: true, 
};

```

###   src--assets--css--themeFn.scss文件说明
