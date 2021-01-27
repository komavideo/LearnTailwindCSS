各种字号一起看
=============

## 知识点

* 编程显示 Tailwind CSS 2.0 支持的各种字号

## 官网

https://tailwindcss.com/docs/font-size

## 实战演习

```html
<template>
    <div>
        <div class="text-gray-600">
            <header class="mb-5">
                <div class="bg-gray-700 p-4 text-white">你好，Tailwind CSS.</div>
            </header>
            <main class="container mx-auto">
                <h1 class="text-2xl">小马学Tailwind CSS</h1>
                <hr>
                <!-- 循环各种字号 Start -->
                <ul>
                    <li v-for="fontsize in list">
                        <div :class="fontsize">Tailwind CSS</div>
                    </li>
                </ul>
                <!-- 循环各种字号 End -->
            </main>
            <footer class="mt-5">
                <div class="bg-gray-300 p-4 text-black">再见，Bootstrap.</div>
            </footer>
        </div>
    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                list: [
                    'text-xs',
                    'text-sm',
                    'text-base',
                    'text-lg',
                    'text-xl',
                    'text-2xl',
                    'text-3xl',
                    'text-4xl',
                    'text-5xl',
                    'text-6xl',
                    'text-7xl',
                    'text-8xl',
                    'text-9xl',
                ]
            };
        },
    }
</script>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P