Tailwind CSS导入方式 - 自编译方式
===============================

## 知识点

* 采用 自编译方式 方式导入 Tailwind CSS 库

## 实战演习

```bash
# 建立新的WEB项目
$ mkdir myweb
$ cd myweb
$ npm init -y
# 建立一个可定制的CSS样式单
$ mkdir src
$ nano src/mytailwind.css
...
@tailwind base;
@tailwind components;
@tailwind utilities;
...
# 生成配置文件
$ npx tailwindcss-cli@latest init
> tailwind.config.js
...
module.exports = {
    purge: ['./**/*.html'],
    darkMode: false, // or 'media' or 'class'
    theme: {
        extend: {},
    },
    variants: {
        extend: {},
    },
    plugins: [],
}
...
# 编写测试文件
$ nano index.html
# 产品模式编译
$ NODE_ENV=production npx tailwindcss-cli@latest build ./src/mytailwind.css -o ./css/tailwind.css
# 文件测试
$ python3 -m http.server 8000 --bind 127.0.0.1 --directory ./
```

### index.html

```html
<!doctype html>
<html>

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link href="./css/tailwind.css" rel="stylesheet">
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


## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P