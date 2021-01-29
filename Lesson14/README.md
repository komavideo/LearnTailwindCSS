做几个自己用的按钮 - Buttons
==========================

## 知识点

* 统一项目中常用的按钮的样式

## 实战演习

### ./assets/css/tailwind.css

```css
.btn_primary {
    @apply bg-bootstrap_primary text-white font-bold py-2 px-3 rounded cursor-pointer tracking-widest hover:bg-yellow-400;
}
.btn_secondary {
    @apply bg-bootstrap_secondary text-white font-bold py-2 px-3 rounded cursor-pointer tracking-widest hover:bg-yellow-400;
}
.btn_success {
    @apply bg-bootstrap_success text-white font-bold py-2 px-3 rounded cursor-pointer tracking-widest hover:bg-yellow-400;
}
.btn_danger {
    @apply bg-bootstrap_danger text-white font-bold py-2 px-3 rounded cursor-pointer tracking-widest hover:bg-yellow-400;
}
.btn_info {
    @apply bg-bootstrap_info text-white font-bold py-2 px-3 rounded cursor-pointer tracking-widest hover:bg-yellow-400;
}
```

### about.vue

```html
<button>确定</button>
<button class="btn_primary">确定</button>
<button class="btn_secondary">确定</button>
<button class="btn_success">确定</button>
<button class="btn_danger">确定</button>
<button class="btn_info">确定</button>
```

## 课程文件

https://github.com/komavideo/LearnTailwindCSS

## 小马视频频道

http://komavideo.com

## 小马部落

https://discord.gg/VSKw72P