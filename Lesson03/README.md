Tailwind CSS导入方式 - Nuxt.js
=============================

## 知识点

* 采用 Nuxtjs 集成的方式导入 Tailwind CSS 库

## 官网

https://tailwindcss.com/docs/guides/nuxtjs

## 实战演习

```bash
# 新建工程
#   注意：不要选择TailwindCSS，因为那个不支持2.0
$ npx create-nuxt-app myweb
$ cd myweb
$ npm install -D @nuxtjs/tailwindcss tailwindcss@npm:@tailwindcss/postcss7-compat @tailwindcss/postcss7-compat "postcss@^7" "autoprefixer@^9"
# 设置 nuxt.js, 追加 tailwindcss, 外置 css
$ nano nuxt.config.js
...
  buildModules: ['@nuxtjs/tailwindcss'],
...
  build: {
    extractCSS: true,
  }
...
# 初始化tailwindcss
$ npx tailwindcss init
> tailwind.config.js
# 修改编译模式，保证产品环境最小化
$ nano tailwind.config.js
...
module.exports = {
    purge: [
        './components/**/*.{vue,js}',
        './layouts/**/*.vue',
        './pages/**/*.vue',
        './plugins/**/*.{js,ts}',
        './nuxt.config.{js,ts}',
    ],
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
# 建立./assets/css/tailwind.css
$ mkdir ./assets/css
$ nano ./assets/css/tailwind.css
...
/* ./assets/css/tailwind.css */
@tailwind base;
@tailwind components;
@tailwind utilities;
...
# 编写一个测试页
$ nano pages/about.vue
# 运行测试
$ npm run dev

Done.
```

### pages/about.vue

```html
<template>
  <div>
    <div class="text-gray-600">
      <header class="mb-5">
        <div class="bg-gray-700 p-4 text-white">Helo world.</div>
      </header>
      <main class="container mx-auto">
        <div class="text-center text-5xl">我的内容我做主！</div>
        <hr class="my-5" />
        <div class="flex justify-center">
          <img src="https://raw.githubusercontent.com/komavideo/LearnTailwindCSS/main/tailwindcss.png"
            class="shadow-lg border my-5">
        </div>
      </main>
      <footer class="mt-5">
        <div class="bg-gray-300 p-4 text-black">你好，Tailwind CSS。</div>
      </footer>
    </div>
  </div>
</template>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P