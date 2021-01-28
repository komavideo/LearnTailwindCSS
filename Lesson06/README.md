定制自己的Tailwind CSS - tailwind.config.js
==========================================

## 知识点

* 使用 tailwind.config.js 文件定制自己的 CSS 主题样式

## 官网

https://tailwindcss.com/docs/configuration

## 实战演习

### 生成 tailwind.config.js

```bash
$ npx tailwindcss init --full
```

### tailwind.config.js

```javascript
// fontSize
    komabig: ['10rem', { lineHeight: '10rem' }],
...
// 定制一个新的主题
theme: {
    extend: {
      colors: {
        bootstrap_primary: '#0d6efd',
        bootstrap_secondary: '#6c757d',
        bootstrap_success: '#198754',
        bootstrap_danger: '#dc3545',
        bootstrap_info: '#0dcaf0',
      }
    },

```

### about.vue

```html
<div class="text-komabig">小马大字体</div>
<div class="bg-bootstrap_primary text-white">像我么</div>
<div class="bg-bootstrap_success text-white">像我么</div>
<div class="bg-bootstrap_danger text-white">像我么</div>
```

## 重新整理一下 tailwind.config.js, 保持维护的代码简洁

```bash
$ npx tailwindcss init
```

### tailwind.config.js

```javascript
module.exports = {
    purge: [],
    darkMode: false, // or 'media' or 'class'
    theme: {
        extend: {
            colors: {
                bootstrap_primary: '#0d6efd',
                bootstrap_secondary: '#6c757d',
                bootstrap_success: '#198754',
                bootstrap_danger: '#dc3545',
                bootstrap_info: '#0dcaf0',
            },
            fontSize: {
                komabig: ['10rem', { lineHeight: '10rem' }],
            }
        },
    },
    variants: {
        extend: {},
    },
    plugins: [],
}
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P