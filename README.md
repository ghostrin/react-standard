
## 初级版
基于react webpack（1.13） react-route(2.8)

## 技术栈：
* ES6
* React
* React-dom
* React-Redux
* Redux
* React-Router
* antd-mobile
* sass、less
* reqwest ajax模块  减少AJAX请求的次数，将考虑使用：Relay和Falcor
* ui库 基于ant-design
* 或者采取[react-css-modules](https://github.com/gajus/react-css-modules) 
* mockjs (完美模拟ajax请求)

## 辅助开发插件
* redux-thunk   action转函数
* redux-logger
* redux-devtools(默认是关闭的注释掉了，如果要用请自行放开,一个是main.jsx，一个是config文件夹下面的store.dev.jsx)

## 高清自适应样式配置
* 添加util.scss文件
* 高宽使用px2Rem( 这里面写正常的PX就好了 ) 进行px转rem , 例如 width:px2Rem(100px);
* 字体实用 @include px2px( 这里写大小就好了不带PX )  , 例如：@include px2px(18);


## 下载

  git clone https://github.com/ghostrin/react-standard.git

  cd react-standard

  npm install

## 目录介绍

```
├── build /                         # 打包的文件目录
├── config /                        # webpack配置
├—— node_modules /                  # npm安装依赖目录
├── src /                           # 开发目录
│   └── app.jsx                     # 项目的整体入口文件, 配置插件
├── .babelrc                        # Babel 配置
├── .editorconfig                   # 统一编辑器配置
├── .env                            # 启动项目自定义端口配置文件
├── .eslintrc.js                    # ES( js / jsx ) 语法纠错
├── .eslintignore                   # 纠错忽略 配置
├── .gitignore                      # git忽略 配置
├── LICENSE                         # GPL3.0
├── package-lock.json               # NPM 依赖包 版本锁
├── package.json                    # 项目 配置
├── README.md                       # 项目 说明
└── yarn.lock                       # Yarn 依赖包版本锁
```

## 安装步骤
* 先装node，验证是否安装好，node -v
* 在安装webpack全局 , cnpm/npm install webpack@1.13.2 -g
* 然后切换到项目文件夹，执行cnpm/npm install


## 运行（nodejs 6.0+）
```
 npm run dev (正常编译模式)

 npm run hot (热替换编译模式)

 访问 http://localhost:8088

 npm run dist （发布生产版本，对代码进行混淆压缩，提取公共代码，分离css文件）
```

