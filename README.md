# vue-3

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## 项目结构

├──src
   ├── components
   │   └── Test.vue
   └── store
       ├── index.js
       └── modules
           ├── male.js
           └── female.js

## 配置
本机版本：Vue CLI v3.0.4

本项目为 Vue2项目

## 常用依赖

### vue-router  
Vue Router 是 Vue.js 官方的路由管理器。它和 Vue.js 的核心深度集成，让构建单页面应用变得易如反掌。
选择指定版本安装，
npm install --legacy-peer-deps vue-router@4.0.13  
若报错则 ： npm install vue-router@3.1.3 --save-dev

### axios   npm install --save axios vue-axios
用于发起Ajax请求，设置拦截请求和响应等
axios是基于promise的HTTP库，可以使用在浏览器和node.js中，它不是vue的第三方插件
vue-axios是axios集成到Vue.js的小包装器，可以像插件一样安装:Vue.use(vueAxios);

### vuex
Vuex是一个专为Vue.js应用程序开发的状态管理模式；它采用集中式存储管理应用的所有组件的状态，并以相应的规则保证状态以一种可预测的方式发生变化。Vuex可以管理复杂应用的数据状态，比如兄弟组件的通信、多层嵌套的组件的传值等等。
npm install vuex@next --save

### element ui
Element，一套为开发者、设计师和产品经理准备的基于 Vue 2.0 的桌面端组件库
npm uninstall element-plus  //卸载
npm install element-plus --save
npm install element-plus@版本号    //例 npm install element-plus@2.1.6
vue add element-plus
cnpm install node-sass
npm i element-ui
### echarts 
ECharts 是一个使用 JavaScript 实现的开源可视化库，涵盖各行业图表，满足各种需求 （注：使用Apache版的）
npm uninstall echarts  //卸载
npm install echarts@4.7.0 --save    //安装指定版本 4.9版本下有地图，5.0版本以上失去这个功能，想要别的版本把@后的版本号改掉就行
安装不同版本
npm install echarts4@npm:echarts@4
npm install echarts5@npm:echarts@5
引入方式
import * as echarts from 'echarts5'
import echarts from 'echarts4'

### less    npm add less less-loader --dev
Less 是一门 CSS 预处理语言，它扩展了 CSS 语言，增加了变量、Mixin、函数等特性，使 CSS 更易维护和扩展
注意这里有个坑，less 和 less-loader 必须写到 devDependencies 里面，不然项目运行会报错

### less-loader
处理scss，将less编译为css

### abel-plugin-syntax-dynamic-import
路由懒加载时用到的组件，把不同路由对应的组件分割成不同代码块，然后当路由被访问时才加载对应组件

### v-distpicker
省市区/县级联选择插件，就是用来选择省、市、区的
