Tailwind CSS 课程介绍
====================

## 课程宗旨

Tailwind CSS 是一个工具集 CSS 框架，可以帮助您快速实现定制化的网站设计，让我们一起学习一下把。

+ No : Bootstrap
+ Yes: Tailwind CSS

## 官方网站

https://tailwindcss.com/

### Github

https://github.com/tailwindlabs/tailwindcss

### Tailwind Toolbox

https://www.tailwindtoolbox.com/

## 使用版本

+ v2.0.2

## 基础知识

+ HTML5
+ CSS/CSS3
+ Javascript

## 开发工具

1. Visual Studio Code(推荐)
2. Brackets/ATOM
3. nano/vim

## 浏览器

1. Chrome(推荐)
2. FireFox
3. MS Edge

## 视频计划

* 每个视频只包括一个知识点，并控制在3-5分钟之内（甚至更短，但经常超时）

## CDN导入

```html
<!doctype html>
<html>

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link href="https://unpkg.com/tailwindcss@2.0.2/dist/tailwind.min.css" rel="stylesheet">
</head>

<body>

    <div class="text-gray-600">
        <header class="mb-5">
            <div class="bg-gray-700 p-4 text-white">Helo world.</div>
        </header>
        <main class="container mx-auto">
            <div class="text-center text-5xl">我的内容我做主！</div>
            <hr class="my-5" />
            <div class="flex justify-center">
                <img src="https://raw.githubusercontent.com/komavideo/LearnTailwindCSS/main/tailwindcss.png" class="shadow-lg border my-5">
            </div>
        </main>
        <footer class="mt-5">
            <div class="bg-gray-300 p-4 text-black">你好，Tailwind CSS。</div>
        </footer>
    </div>
</body>

</html>
```

## http.server

```bash
# 文件测试
$ python3 -m http.server 8000 --bind 127.0.0.1 --directory ./
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P