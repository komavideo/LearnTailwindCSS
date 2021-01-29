变换与动画 - transition and animations
=====================================

## 知识点

* 使用纯CSS实现简单动画变换效果

## 官网

https://tailwindcss.com/docs/transition-property

## 实战演习

```html
<div class="flex flex-col">
    <div class="flex justify-center">
        <button class="btn_primary mx-1">确定</button>
        <button class="btn_secondary mx-1">确定</button>
        <button class="btn_success mx-1">确定</button>
        <button class="btn_danger mx-1">确定</button>
        <button class="btn_info mx-1">确定</button>
    </div>
    <div class="flex justify-center pt-5">
        <!-- 变换效果 -->
        <button class="btn_primary mx-1 transform ease-in duration-300">确定</button>
        <button class="btn_secondary mx-1 transform ease-out duration-700 hover:scale-125 py-3 px-6">确定</button>
        <button class="btn_success mx-1">
            <svg class="animate-spin h-5 w-5 text-white inline-block" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
            </svg>                            
            确定</button>

        <div class="relative inline-flex rounded-md shadow-sm mx-1">
            <button class="btn_danger">确定</button>
            <span class="flex absolute h-3 w-3 top-0 right-0 -mt-1 -mr-1">
                <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-yellow-400 opacity-75"></span>
                <span class="relative inline-flex rounded-full h-3 w-3 bg-yellow-500"></span>
            </span>
        </div>

        <button class="btn_info mx-1" @click="clickMe">确定</button>
    </div>
</div>
```

```javascript
<script>
    export default {
        data: function () {
            return {
                list: []
            };
        },
        methods: {
            clickMe: function() {
                alert('I like Tailwind CSS.')
            }
        }
    }
</script>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P