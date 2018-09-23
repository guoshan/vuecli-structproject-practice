# travel-self

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
## 常用点记载
### 图片宽高等比例显示 假设宽高比例为31.25% 图片容器显示为下面两种 
``` bash
    .wrapper
        overflow:hidden
        width:100%
        height:0
        padding-bottom:31.25%

    .wrapper
        width:100%
        height:31.25vw
```