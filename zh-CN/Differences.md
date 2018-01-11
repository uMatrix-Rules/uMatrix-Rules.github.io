## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava---toc)

你可能想知道为何在即使你已经在 uBlock Origin 控制台中勾选 `高级用户模式` 并手动添加永久规则 `* * 3p block` 、`* * 3p-script block` 、`* * 3p-frame block` 的情况下，uMatrix 仍然是有必要使用的。

通过添加这些规则，uBlock Origin 就会切换到[困难模式](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode)。

总体而言，uMatrix 专注于 `元素控制` 而 uBlock Origin 能更好地处理 `域名控制` 与 `精细请求过滤` 的功能。具体解释为：

#### 元素控制

打开 YouTube 任意一个视频播放页，uMatrix 或者 uBlock Origin [困难模式](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode)都会拦截下方评论区。恢复显示评论区的办法如下：

- 打开 uBlock Origin 工具栏弹窗，点击放行该页来自于 `google.com` 的网络请求。在此情况下，来自于 `google.com` 的**任意类型**的页面请求都会被放行。
- 打开 uMatrix 工具栏弹窗，点击放行来自于 `google.com` 的 `脚本` 与 `cookie`。这样其它来自于 `google.com` 的页面请求类型都会**保持拦截**。

上述任一办法都能恢复使用 YouTube 评论区，然而很明显，uMatrix 有着更有效的 `元素控制` 能力。

#### 精细请求过滤

uBlock Origin 内置大量的规则订阅并且兼容全部 AdBlock Plus 语法。在精细过滤方面 uMatrix 显然有所不足。

就之前的的例子，使用 uMatrix 你能拦截或放行来自于 `google.com` 的全部脚本。但是 uBlock Origin 就能拦截任意数量的脚本。办法很简单，在 uBlock Origin 控制台的 `自定义规则` 选项卡中创建一条规则即可，或者，利用[元素选择器](https://github.com/gorhill/uBlock/wiki/Element-picker)或其它内置工具。

### Reeshoova! - 许可协议

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
除非额外声明，否则本组织中全部内容许可协议均为 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
