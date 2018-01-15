## Vrooboo! Wabbo!!

此处为规则使用知识集合库。

[uMatrix](https://github.com/gorhill/uMatrix) 是一个浏览器扩展，可以根据网络请求的来源、类型、目标等进行点状控制。

---

## Ovagarava - T.O.C.

- [黑名单模式](Blacklist-Mode.md)
- [贡献指引](Guidelines.md)
- [Cookies 控制](Cookies-Control.md)
- [uMatrix 与 uBlock Origin 困难模式之间的区别](Differences.md)
- [临时规则](Temp.md)
- 第三方框架
    - [Google 服务](Google-Services.md)
    - [Video 框架举例](Video-Iframe-Examples.md)
    - [其它](Others.md)
- [uMatrix 按钮功能](Visual.md)

---

## Shagdovala - FAQs

1. 允许加载第三方元素应该遵循什么原则？

    首先应该确保日常浏览中大部分站点功能正常运作，在此基础上，越多元素被拦截效果越好。

2. 仅使用 uMatrix 就足够了吗（还有没有推荐的隐私增强工具）？

    答案是否定的。有些第三方元素同时包含正常站点功能元素与追踪脚本。以下为可能有帮助的例子：
    - [CanvasBlocker](https://github.com/kkapsner/CanvasBlocker)：无忧隐私防护
    - [Cookie-AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete)：谨慎开启`主动模式`
    - [Decentraleyes](https://decentraleyes.org/)：强烈推荐
    - [Don't Fuck With Paste](https://addons.mozilla.org/firefox/addon/don-t-fuck-with-paste/)：可能破坏一些特定的页面
    - [HTTPS Everywhere](https://www.eff.org/https-everywhere)：占用大量 RAM 并且很有可能有严重性能问题
    - [Neat URL](http://hugsmile.eu/)
    - [NoProfile](https://addons.mozilla.org/firefox/addon/noprofile/)：某些站点可能表现异常，尤其是包含大量鼠标悬浮特效时
    - [uBlock Origin](https://github.com/gorhill/uBlock)：完美组合
    - [URL Tooltip WE](https://addons.mozilla.org/firefox/addon/url-tooltip-we/)

    此外，如果你使用 [Mozilla Firefox](https://www.mozilla.org/firefox/all/)，除 battery API 已移除以保护隐私，同时建议转到：

    - `about:preferences#privacy`
        - 在 `历史` 一节，在 `接受第三方 cookies` 一项中选择 `从不`；勾选 `Firefox 退出时清理历史`，在其中的更多选项中至少建议勾选 `缓存`、`站点设置` 与 `离线网站数据`。 
        - 在 `追踪保护` 一节，选中两个 `总是` 。
        - 在 `权限` 一节，勾选 `阻止无障碍服务接入浏览器` 。
        - 在 `安全` 一节，**取消勾选** `拦截危险的下载与站点`：这一功能使用 Google Safe Browsing API 并会时刻追踪用户。如有必要，请使用专业反病毒软件。
    - `about:preferences#search`
        - 在 `默认搜索引擎` 一节，**取消勾选** `在地址栏中显示搜索建议`：搜索引擎能因此收集信息。如有必要，请使用不记录搜索的引擎作为替代，比如 DuckDuckGo。

3. 如何捐助？

    [组织所有人](https://github.com/Rictusempra)无意接受任何捐助。您可以询问[其他成员](https://github.com/orgs/uMatrix-Rules/people)是否有意愿。

4. 本站有些奇怪的词是什么意思？

    它们是一个叫 `LOL` 的 MMORPG 中的一个叫`纳尔`的角色台词。你可以[在这里](http://leagueoflegends.wikia.com/wiki/Gnar/Quotes)找到全部它的台词。

## Gnar gada! - 使用方法

1. 首选选择适合自己的规则类别：[domain](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain) 或者 [site](https://github.com/uMatrix-Rules/uMatrix-Rules-Site)。建议选择后者。将 `rules.text` 文件保存到本地或者直接在浏览器中打开并复制全部内容。
2. 打开 uMatrix 控制台
3. 转到 `自定义规则` 选项卡
4. 导入规则：
   - 点击 `从文件导入...` 并选择你保存的文件，或者；
   - 点击 `编辑` 并从剪贴板粘贴
5. 按需求编辑或点击 `保存`，然后点击 `提交`

## Shubbanuffa - 使用须知

1. 仅保证大部分站点功能正常。使用须自负风险。
2. 当需要提交站点异常时，请在[对应的 repository](https://github.com/uMatrix-Rules) 新建一个 issue：
    - 给出具体的 URL
    - 附注 uMatrix 与浏览器 version
    - 附注你自行创建的规则。如已修改默认设置，须一并指出
    - 当提交的网站需要一个账号的时候，你必须首先将一个可用的账号发送到[组织邮箱](lolipopplus@protonmail.com)。发送即视为信任[组织所有人](https://github.com/Rictusempra)。
3. 当遇到以下情况导致的站点异常时不会予以处理：
    -  站点功能内容被内置订阅拦截
    -  站点功能异常来由并非 uMatrix 规则或者 uMatrix 自身设置
    -  当该站点符合以下任意情况之一时：
        -  使用不受信任的 CA 签发的证书
        -  **大部分**内容均为色情内容
        -  被报告为危险站点
        -  并非托管于公共服务的个人博客站点
    -  与插件相关，例如 Adobe Flash
    -  其它 uMatrix [README](https://github.com/gorhill/uMatrix/blob/master/README.md) 或 [wiki](https://github.com/gorhill/uMatrix/wiki) 中已明确的问题

---

### Reeshoova! - 许可协议

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
除非额外声明，否则本组织中全部内容许可协议均为 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
