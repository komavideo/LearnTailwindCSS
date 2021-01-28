绝对布局和相对布局
================

## 知识点

* 绝对布局和相对布局, 实现图层叠加

## 实战演习

```html
<div class="flex justify-around bg-gray-200 p-5">
    <div class="bg-white rounded overflow-hidden shadow-md">
        <img src="/gtagirl.png" alt="gta" class="w-80 object-cover">
        <div class="p-2">
            <div class="font-bold text-lg">GTA女孩</div>
            <div class="text-gray-500 text-sm">GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
        <div class="p-2 border-t border-gray-200">
            <div class="flex justify-end text-xs text-red-500">发卖日：2013年9月17日</div>
        </div>
    </div>
    <!-- Card设计 -->
    <div class="bg-white rounded overflow-hidden shadow-md relative">
        <img src="/gtagirl.png" alt="gta" class="w-80 object-cover">
        <div class="p-2">
            <div class="font-bold text-lg">GTA女孩</div>
            <div class="text-gray-500 text-sm">GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
        <div class="p-2 border-t border-gray-200">
            <div class="flex justify-end text-xs text-red-500">发卖日：2013年9月17日</div>
        </div>
        <div class="bg-yellow-300 rounded-full absolute top-0 ml-1 mt-1">
            <span class="text-red-600 font-bold p-1 text-3xl">5.0</span>
        </div>
    </div>
    <!-- 评分居右 -->
    <div class="bg-white rounded overflow-hidden shadow-md relative">
        <img src="/gtagirl.png" alt="gta" class="w-80 object-cover">
        <div class="p-2">
            <div class="font-bold text-lg">GTA女孩</div>
            <div class="text-gray-500 text-sm">GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
        <div class="p-2 border-t border-gray-200">
            <div class="flex justify-end text-xs text-red-500">发卖日：2013年9月17日</div>
        </div>
        <div class="bg-yellow-300 rounded-full absolute top-0 right-0 mr-1 mt-1">
            <span class="text-red-600 font-bold p-1 text-3xl">5.0</span>
        </div>
    </div>
</div>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P