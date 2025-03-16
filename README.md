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
-   ::after 伪元素必须设置 content 属性（即使为空值如 content: ""），否则不会显示。该伪元素可以被视为是元素的最后一个子元素，并且可以设置宽高、位置等属性（例如 height:100%时，伪元素会占满整个元素的高度）。同样的规则也适用于 ::before 伪元素。
-   animation-fill-mode: backwards 表示动画开始前，元素会应用动画第一帧的样式，animation-fill-mode: forwards 表示动画结束后，元素会应用动画最后一帧的样式
-   3 pillars:Responsive design, Maintainable and scalableWeb, code performance
-   Atomic design pattern: Atoms, Molecules, Organisms, Templates, Pages
-   BEM: Block, Element, Modifier, 元素和修饰符之间用--链接，如 .btn--primary， 模块和元素之间用\_\*2 链接，如 .header\_\*2logo-box
-   优先使用 max-width 代替 width
-   属性选择器可以用于代码复用
-   使用 clip-path 时，会使 overflow: hidden 失效，可以手动加 border-radius
-   shape-outside 属性可以用于设置元素的形状。这个属性严格要求元素 float，并且有宽度个高度
-   响应式设计中，图片必须有一个宽度
-   opacity:0 会使元素不可见，但是仍然占据空间，而 visibility:hidden 会使元素不可见，并且不占据空间。但是后者不能展示动画效果。可以通过 opacity:0 和 visibility:hidden 配合使用来实现动画效果。
-   author 配合 target 可以实现 modal 的显示隐藏效果
-   媒体查询中的 rem 和 em 不受根字体大小的影响，他们总是等于浏览器字体大小，默认值为 16px。rems 在不同浏览器之间兼容性较差，在媒体查询中使用 ems 是更好的选择（几年前）
-   媒体查询放置的顺序有讲究:大的放在小的前面，否则小的永远不会被应用
