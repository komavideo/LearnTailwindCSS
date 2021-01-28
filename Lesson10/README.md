做出我们自己的卡片 - Card
======================

## 知识点

* 活用 Tailwind CSS 做出我们自己的卡片布局

## Bootstrap卡片样式

https://getbootstrap.com/docs/5.0/components/card/

## 实战演习

```html
<div class="flex justify-around bg-gray-200 p-5">
    <div>
        <img src="/gtagirl.png" alt="gta" class="w-80">
        <div>
            <div>GTA女孩</div>
            <div>GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
    </div>
    <!-- Card设计 -->
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
</div>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P