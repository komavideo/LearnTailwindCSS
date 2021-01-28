引入我要的字体 - font, fontFamily
===============================

## 知识点

* 在项目中加入第三方的字体

## 官网

https://fonts.google.com/

## 实战演习

首先在Google Fonts中选取要使用的字体。

### ./assets/css/tailwind.css

```css
@import url('https://fonts.googleapis.com/css2?family=Zhi+Mang+Xing&display=swap');

@tailwind base;
@tailwind components;
@tailwind utilities;
```

### tailwind.config.js

```javascript
...
    fontSize: {
        komabig: ['10rem', { lineHeight: '10rem' }],
    },
    fontFamily: {
        komafont: ['Zhi Mang Xing']
    }
...
```

### about.vue

```html
<div class="font-komafont text-komabig">小马大字体</div>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P