# vue-particle

> vue-particles可以生成类似于星座图的点和线，并且能与用户的鼠标事件产生互动。

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

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


## 使用教程 ：

``` bash
npm install vue-particles --save-dev  
```

## 局部安装完 vue-particles 后，在 main.js 引入，并在vue项目中使用。

``` bash
import VueParticles from 'vue-particles'

Vue.use(VueParticles)  
```

## 成功引入后，以一个简单的例子作为demo。 直接在App.vue中添加vue-particles：

``` bash
<template>  
    <div id="app">
      <vue-particles color="#dedede"></vue-particles>
    </div>
</template>
 ```
 
 ## 通过设置vue-particles选项来实现一个比较完整的例子：
 
 ``` bash
<template>  
    <div id="app">
      <vue-particles
        color="#dedede"
        :particleOpacity="0.7"
        :particlesNumber="80"
        shapeType="circle"
        :particleSize="4"
        linesColor="#dedede"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="3"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="true"
        clickMode="push"
      >
      </vue-particles>
    </div>
 </template>
```

## 属性分别如下所示：

``` bash
color: String类型。默认'#dedede'。粒子颜色。

particleOpacity: Number类型。默认0.7。粒子透明度。

particlesNumber: Number类型。默认80。粒子数量。

shapeType: String类型。默认'circle'。可用的粒子外观类型有："circle","edge","triangle", "polygon","star"。

particleSize: Number类型。默认80。单个粒子大小。

linesColor: String类型。默认'#dedede'。线条颜色。

linesWidth: Number类型。默认1。线条宽度。

lineLinked: 布尔类型。默认true。连接线是否可用。

lineOpacity: Number类型。默认0.4。线条透明度。

linesDistance: Number类型。默认150。线条距离。

moveSpeed: Number类型。默认3。粒子运动速度。

hoverEffect: 布尔类型。默认true。是否有hover特效。

hoverMode: String类型。默认true。可用的hover模式有: "grab", "repulse", "bubble"。

clickEffect: 布尔类型。默认true。是否有click特效。

clickMode: String类型。默认true。可用的click模式有: "push", "remove", "repulse", "bubble"。

```

## 效果

放张静态图片大致感受下粒子效果，实际效果是动态的，包括跟着鼠标移动等动效，可以通过上面提到的参数自己进行个性化配置。


![1.png](https://github.com/lulin1/vue-particles/blob/master/static/img/1.png)


