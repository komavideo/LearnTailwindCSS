复用自己的Card样式 - @apply
=========================

## 知识点

* 把常用的样式组合在一起，形成自己的样式

## 官网

https://tailwindcss.com/docs/functions-and-directives#apply

## 实战演习

```html
<div class="flex justify-around bg-gray-200 p-5">
    <div class="bg-white rounded overflow-hidden shadow-md relative">
        <img src="/gtagirl.png" alt="gta" class="w-80 object-cover">
        <div class="p-2">
            <div class="font-bold text-lg">GTA女孩</div>
            <div class="text-gray-500 text-sm">GTA6啥时发卖？钱包我都准备好了。</div>
        </div>
        <div class="p-2 border-t border-gray-200">
            <div class="flex justify-end text-xs text-red-500">发卖日：2013年9月17日</div>
        </div>
        <div
            class="bg-yellow-300 rounded-full text-red-600 font-bold p-1 text-3xl absolute top-0 ml-1 mt-1">
            <span>5.0</span>
        </div>
    </div>
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

### ./assets/css/tailwind.css

```css
.card {
    @apply bg-white rounded overflow-hidden shadow-md relative;
}
.card_image {
    @apply w-80 object-cover;
}
.card_badge {
    @apply bg-yellow-300 rounded-full text-red-600 font-bold p-1 text-3xl absolute top-0 ml-1 mt-1;
}
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P