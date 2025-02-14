# Learnings

-   所有跟字体有关的 css 设置，全部放在 body 标签上，不单独放在其他标签中
-   line-height 的数值一般表示的是倍数，比如 1.5 表示 150%（预定义的 1.5 倍）
-   通常使用 background-image 来实现图片颜色渐变
-   padding 的 4 个值，分别表示上、右、下、左（顺时针）
-   clip-path: polygon 中可以指定许多个点，表示一个多边形
-   对于 img 这种 inline 元素来说，使用时最好套一层 div，方便定位等操作
-   alt 属性：当图片加载失败时，会显示 alt 中的内容；当图片被搜索引擎抓取时，会显示 alt 中的内容（SEO 优化）
-   span 元素常常用来展示不同样式的文本
-   span 元素默认是 inline 元素
-   block 元素默认占满宽度（独占一行），并且在其前后会有换行符
-   使用 animation 时，最好只使用 2 个属性，即 opacity 和 transform，它们是浏览器特殊优化过的
-   backface-visibility 本来是用于隐藏元素的背面（旋转时不可见），不过它也可以用于 animation 中的元素异常抖动问题（不清楚原理，但可行）
-   文本级元素（如 span、a、strong、em 等）默认是 inline 元素，而结构级元素（如 div、p、h1-h6 等）默认是 block 元素。内联元素无法设置宽高，而结构级元素可以设置宽高。内联元素会在同一行内紧密排列（表现为入侵），而块级元素会独占一行。可以使用 display: inline-block 来同时获得内联和块级元素的特性。
-   伪类:active 表示元素被点击时（按下鼠标并松开）的状态
