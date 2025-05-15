---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /bg.png
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
# seoMeta:
#  ogImage: https://cover.sli.dev
---

# Web编辑器

<p class="text-sm pt-6 align-left" >
  <div>part1：架构管理平台中的应用</div>
  <div>part2：开源文档编辑的能力</div>
</p>

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  按空格键查看下一页 <carbon:arrow-right />
</div>

<div class="abs-br m-4 text-xl">
 From Mogy
</div>

---
transition: fade-out
---

# 需求

1. 基础功能齐全（本身提供一些开箱即用的功能，减少开发的成本）
   1. 字体设置（包括字体、颜色、大小、标题）
   2. 有序列表与无序列表
   3. 插入（表格、图片、链接）
   4. ...等等
2. 可拓展性高（支持以自定义插件的形式增加工具栏功能，和内容区域的功能）
3. 工具栏和编辑区域能分开展示（布局自定义）  &#x20;
4. 拆分模块编辑（块编辑器）
5. 选择插入图片时，可以回调我们系统中的接口，列出可选图片插入（自定义插入图片功能）
6. 提供图片编辑按钮，可以跳转到我们系统编辑（自定义插入图片功能）
7. 对图片的插入和删除可以给我们事件，以便管理图片与文档的关系
8. 支持导入数据快速生成表格（数据库导入，自定义表格功能）
9. 对接AI，编辑时可以菜单支持我们插入自动生成的文本（AI功能）

---
transition: slide-up
level: 2
---

# Web编辑器在架构管理中的应用

<div my-3>现阶段功能：</div>

- 📝 **常规编辑功能** - 字体样式、标题、列表、表格等等
- 🛠 **自定义模版** - 根据公司文档模板自定义
- 🗳️ **数据库导入** - 直接连接数据库导入表结构数据
- 📸 **插入图片** - 导入架构管理平台中的图，支持二次编辑

<br>
<br>
<br>
<br>

Powered by [架构管理平台](https://eamp.cmschina.com.cn)

---

# 开源编辑器的能力

<div grid="~ cols-2 gap-4">
<div>

本质：一个可编辑的`<div></div>`。


```html
  <div contenteditable="true" >
    <p>这是一个段落</p>
  </div>
```

<!-- ./components/Counter.vue -->
<Div v-click :count="10" m="t-5" />

<div v-click class="text-teal-600 my-4 text-2xl">contenteditable + HTML + CSS</div>

<div v-click>这就意味着网页上能展示的元素，编辑器中绝大多数都能展示，例如：文本、mp3/mp4、Image等等</div>

</div>
<div>

<div  v-click>类型：L0 -> L1 -> L2 </div>

<img
  v-click
  class=" w-full"
  src="/images/image_ZvD0-yeQwR.png"
  alt=""
/>

</div>
</div>

<!--
Presenter note with **bold**, *italic*, and ~~striked~~ text.

Also, HTML elements are valid:
<div class="flex w-full">
  <span style="flex-grow: 1;">Left content</span>
  <span>Right content</span>
</div>
-->



---
transition: fade-out
---

# 优秀的商业产品

- 📝 **语雀** - [https://www.yuque.com/](https://www.yuque.com/)
- 🎨 **wolai** - [https://www.wolai.com/](https://www.wolai.com/)
- 🧑‍💻 **notion** - [https://www.notion.com/](https://www.notion.com/)
- 🤹 **Obsidian** - [https://obsidian.md/](https://obsidian.md/)
- 🎥 **WPS** - [https://www.kdocs.cn/](https://www.kdocs.cn/)


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

