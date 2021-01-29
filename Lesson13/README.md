网格布局 - Grid
==============

## 知识点

* 使用网格布局，规范页面显示内容

## 官网

https://tailwindcss.com/docs/grid-template-columns

## 实战演习

### 布局Card内容显示

```html
<div class="bg-gray-200 p-5 grid grid-cols-1 md:grid-cols-3 xl:grid-cols-4 gap-5">
<!-- <div class="bg-gray-200 p-5"> -->
    <!-- Card设计 -->
    <div class="card">
        <img src="/gtagirl.png" alt="gta" class="card_image">
        <div class="p-2">
            <div class="font-bold text-lg">GTA女孩</div>
            <div class="text-gray-500 text-sm">GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
        <div class="p-2 border-t border-gray-200">
            <div class="flex justify-end text-xs text-red-500">发卖日：2013年9月17日</div>
        </div>
        <div class="card_badge">
            <span>5.0</span>
        </div>
    </div>
</div>
```

### 页面分割布局

```html
<!-- 左右菜单栏布局 -->
<div>
    <div>菜单栏</div>
    <div>主内容区</div>
</div>
<!-- 按1/3，2/3比例分配功能页面区 -->
<div class="grid grid-cols-3">
    <div class="bg-gray-300 col-span-1">菜单栏</div>
    <div class="bg-red-300 col-span-2">主内容区</div>
</div>
<!-- 响应式分配:md以上布局采用1/3,2/3样式 -->
<div class="grid md:grid-cols-3">
    <div class="bg-gray-300 md:col-span-1">菜单栏</div>
    <div class="bg-red-300 md:col-span-2">主内容区</div>
</div>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P