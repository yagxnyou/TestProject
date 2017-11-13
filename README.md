
##本项目主要目的属于自我学习，并不会有商业行为 by yagxnyou

使用到的技术栈：vue + vue-resource + vue-router + vuex(spa必备) + element-ui + ES6 + webpack + npm 

[测试地址](https://lss5270.github.io/vue-admin-spa-demo)


## 功能(全部数据进行本地json模拟)
- 系统说明
- 登录/注销
- 密码修改
- 个人主页
- 头像上传
- 权限验证
- 修改权限
- 侧边栏
- 面包屑
- 富文本编辑器
- 切换主题（点击头像下拉）
- 表单校验、提交
- 列表增删改查、排序、导出(后台管理系统基本功能)
- 401，404重定向页面
- 导出excel
- views-tab
- PC端更多功能即将开放……
- 等后面有空再给大家开源一个vue的移动端项目，嘿嘿^_^

## 开发
```bash
    # 克隆代码
    git clone https://github.com/lss5270/vue-admin-spa.git
    # 安装依赖
    npm install
    #or 直接解压node_modules.7z到当前位置 （比较适合新手）。

    # 本地开发 开启服务
    npm run dev
    #or 直接双击start.bat（比较适合新手）
```
```[下载node_modules](http://pan.baidu.com/s/1eSL4I8y)
```

浏览器访问 http://localhost:2017

## 发布
```bash
  
    # 构建生产环境
    npm run build:prod
    #or 直接双击build.bat（比较适合新手）
```
## 模拟运行正式环境
```bash
    # nginx环境下运行
    1.准备nginx环境，自行到nginx官网（https://nginx.org/）下载，并解压
    2.双击build.bat后根目录生成一个dist包，把dist整个文件夹拷贝到nginx解压后的html下
    3.启动nginx服务：双击nginx.exe
    4.访问入口：http://localhost/dist/index.html
    ………
    
    8.关闭nginx服务：直接删进程
    
    # tomcat环境下运行
    参照nginx步骤即可
```

## 关于图标
```
    本项目使用了两套图标系统，具体使用方法参照以下官方链接:
    1.http://element.eleme.io/#/zh-CN/component/icon
    2.http://fontawesome.io/icons/
    使用方法：
    a.在index.html中引入<link href="//cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.css" rel="stylesheet">
    b.在使用图标的地方放置图标<i class="fa fa-home" aria-hidden="true"></i>
```
## 关于UI系统
```
    由于bootstrap不支持mvvm已弃用，本项目使用了全新的elementUI系统，具体使用方法参照以下官方链接:
    1.http://element.eleme.io/#/zh-CN/component/installation
    
```
## 关于.vue文件中背景图片路径，打包到生产环境路径404的问题修复
```
    具体修复方法，参照Issues中的 #6问题
    
```


## 目录结构
```shell
├── build                      // 构建相关  
├── config                     // 配置相关
├── src                        // 源代码
│   ├── assets                 // 主题 字体等静态资源
│   ├── components             // 全局公用组件。不直接显示
│   ├── global                 // 全局指令
│   ├── filtres                // 全局filter
│   ├── router                 // 路由
│   ├── store                  // 全局store管理
│   ├── utils                  // 全局公用方法
│   ├── view                   // view视图层
│   ├── App.vue                // 入口页面
│   └── main.js                // 入口 加载组件 初始化等
├── static                     // 第三方不打包资源
│   ├── jquery
│   ├── Tinymce                // 富文本
│   ├── dataJson               // 模拟接口json
│   └── theme                  // 主题文件
├── .babelrc                   // babel-loader 配置
├── eslintrc.js                // eslint 配置项
├── .gitignore                 // git 忽略项
├── favicon.ico                // favicon图标
├── index.html                 // html模板
└── package.json               // package.json








