<h1 align=center>OREO 3D</h1>

## 简介

生成并导出一个3D`奥利奥`。

<img width="100%" src="https://raw.githack.com/syt123450/oreo-3d/master/assets/intro.png">

## 功能？

这个`奥利奥`生成器有不少 <b>实（~~沙~~） 用（~~雕~~）</b> 的功能

* 揉一揉`奥利奥`

<img width="100%" src="https://raw.githack.com/syt123450/oreo-3d/master/assets/rolling.gif">

* `奥利奥`出现了，又消失了，再次出现了，然后又消失了。。。

<img width="100%" src="https://raw.githack.com/syt123450/oreo-3d/master/assets/zoom.gif">

* 生成特别的`奥利奥`

<img width="100%" src="https://raw.githack.com/syt123450/oreo-3d/master/assets/generate.gif">

* 打包导出3D`奥利奥`（3D场景，.gltf格式）

## 本地运行

需要本地安装yarn

* 安装依赖

```shell
yarn
```

* 启动本地服务器

```shell
yarn start
```

* 在浏览器端查看

```shell
http://localhost:3000/
```

## 实现简介

主要实现过程：

* Three.js 3D 场景创建

    * 3D 雾化场景增加镜深感
    * 添加平板作为地面接受反光
    * 使用`冯氏材质`提升光感
    * 创建`饼干`对象与`夹心`对象以复用
    * STL Loader 加载模型素材
    * GLTF Exporter 导出可复用场景

* React 项目粘合剂

    * create-react-app 脚手架创建
    * react-toolbox UI 组件
    * react-localization 多语言

## 引用

奥利奥图片生成器 [oreooo](https://github.com/ddiu8081/oreooo)