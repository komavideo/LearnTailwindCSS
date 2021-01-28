使用 Flexbox 布局
================

## 知识点

* 使用 Flexbox 布局安排页面空间与控件

## 官网

https://tailwindcss.com/docs/flex-direction  
https://tailwindcss.com/docs/justify-content  

## Flexbox讲解

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

## 实战演习

```html
<!-- 默认布局 -->
<div class="text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 行布局 -->
<div class="flex flex-row text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 行布局(反转) -->
<div class="flex flex-row-reverse text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 列布局 -->
<div class="flex flex-col text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 列布局(反转) -->
<div class="flex flex-col-reverse text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>

<!-- 对齐内容 - 左对齐 -->
<div class="flex justify-start text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 对齐内容 - 右对齐 -->
<div class="flex justify-end text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 对齐内容 - 居中对齐 -->
<div class="flex justify-center text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 对齐内容 - 平均分布对齐1 -->
<div class="flex justify-between text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 对齐内容 - 平均分布对齐2 -->
<div class="flex justify-around text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 对齐内容 - 平均分布对齐3 -->
<div class="flex justify-evenly text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-10 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-10 bg-bootstrap_danger text-white m-2">3</div>
</div>

<!-- 水平轴对齐 - 原始 -->
<div class="text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-20 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-32 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 水平轴对齐 - 上对齐 -->
<div class="flex items-start text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-20 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-32 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 水平轴对齐 - 中对齐 -->
<div class="flex items-center text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-20 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-32 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 水平轴对齐 - 下对齐 -->
<div class="flex items-end text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-20 bg-bootstrap_success text-white m-2">2</div>
    <div class="w-10 h-32 bg-bootstrap_danger text-white m-2">3</div>
</div>
<!-- 水平轴对齐 - 基准线对齐 -->
<div class="flex items-baseline text-center bg-gray-100 mt-3">
    <div class="w-10 h-10 bg-bootstrap_primary text-white m-2">1</div>
    <div class="w-10 h-20 bg-bootstrap_success text-white m-2 flex  justify-center items-center">2</div>
    <div class="w-10 h-32 bg-bootstrap_danger text-white m-2">3</div>
</div>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P