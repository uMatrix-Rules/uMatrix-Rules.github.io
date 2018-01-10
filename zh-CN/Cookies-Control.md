## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava---toc)

证如 [uMatrix wiki](https://github.com/gorhill/uMatrix/wiki/Cookies) 中所说，uMatrix 会阻止 cookies `遗留在浏览器中`。
遵循以下步骤可以获得更好的效果：

添加规则 `* * cookie block`，意为默认全局阻止 cookies。此后必须要在需要 cookies 的站点手动允许 cookies。以下是一个例子：

    * * cookie block
    google.com accounts.google.com cookie allow
    google.com google.com cookie block

这一情况下，`google.com google.com cookie block` 会阻止来自于 Google 搜索的基于 cookies 的追踪，同时，`google.com accounts.google.com cookie allow` 将保证可以登录一些 Google 的服务。

这一实现位于[此处](https://github.com/uMatrix-Rules/uMatrix-Rules-Site/tree/Strict-Cookies)。

### Reeshoova! - 许可协议

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
除非额外声明，否则本组织中全部内容许可协议均为 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
