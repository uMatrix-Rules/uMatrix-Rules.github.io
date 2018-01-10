## Vrooboo! Wabbo!!

此处为规则使用知识集合库。

[uMatrix](https://github.com/gorhill/uMatrix) 是一个浏览器扩展，可以根据网络请求的来源、类型、目标等进行点状控制。

---

## Ovagarava - T.O.C.

- [黑名单模式](Blacklist-Mode.md)
- [贡献指引](Contributing.md)
- [Cookies 控制](Cookies-Control.md)
- [uMatrix 与 uBlock Origin 高级模式之间的区别](Differences.md)
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
    - [CanvasBlocker](https://github.com/kkapsner/CanvasBlocker)
    - [Cookie-AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete)
    - [Decentraleyes](https://decentraleyes.org/)
    - [Don't Fuck With Paste](https://addons.mozilla.org/firefox/addon/don-t-fuck-with-paste/)：可能破坏一些特定的页面
    - [HTTPS Everywhere](https://www.eff.org/https-everywhere)：占用大量 RAM 并且很有可能有严重性能问题
    - [Neat URL](http://hugsmile.eu/)
    - [NoProfile](https://addons.mozilla.org/firefox/addon/noprofile/)：某些站点可能表现异常，尤其是包含大量鼠标悬浮特效时
    - [uBlock Origin](https://github.com/gorhill/uBlock)
    - [URL Tooltip WE](https://addons.mozilla.org/firefox/addon/url-tooltip-we/)

    此外，如果你使用 [Mozilla Firefox](https://www.mozilla.org/firefox/all/)，除 battery API 已移除以保护隐私，同时建议转到：

    - `about:preferences#privacy`
        - 在 `历史` 一节，在 `接受第三方 cookies` 一项中选择 `从不`；勾选 `Firefox 退出时清理历史`，在其中的更多选项中至少建议勾选 `缓存`、`站点设置` 与 `离线网站数据`。 
        - at `Tracking Protection` section, select both `Always`
        - at `Permissions` section, check `Prevent accessibility services from accessing your browser`.
        - at `Security` section, **uncheck** `Block dangerous and deceptive content`: this uses Google Safe Browsing API and tracks your everywhere. Use pro anti-virus programs instead if necessary.
    - `about:preferences#search`
        - at `Default Search Engine` section, **uncheck** `Show search suggestions in address bar results`: the search engine provider will collect info if this is checked. If you rely on the suggestions, use engines that don't record things instead, e.g. DuckDuckGo.

3. How can I donate?

    [The owner](https://github.com/Rictusempra) has no any will to accept. Check how [other members](https://github.com/orgs/uMatrix-Rules/people) say.

4. What are these strange awkward words on this page?

    They are quotes of a character, `Gnar`, in an MMORPG called `League of Legends`. You may find all quotes [here](http://leagueoflegends.wikia.com/wiki/Gnar/Quotes).

## Gnar gada! - USAGE

1. First, choose a rule level you would prefer, [domain](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain) or [site](https://github.com/uMatrix-Rules/uMatrix-Rules-Site).  It is recommended to choose the latter. Save the `rules.txt` into any local directory, or directly open it in your browser & copy all contents
2. open your uMatrix dashboard
3. navigate to `My rules` tab
4. import the rules:
   - click `Import from file...` and pick the file you just downloaded or;
   - click `Edit` and paste them from clipboard
5. edit as your like and/or click `Save`, and then `Commit`

## Shubbanuffa - BEFORE USING

- I can only ensure most site functions are workable. Use at your own risk.
- If you are expecting my investigation on any specific site, pls open a new issue at [corresponding place](https://github.com/uMatrix-Rules):
    - give a specific URL
    - point out your uMatrix version & broswer version
    - attach your own rules and, if differ from default, your preferences
    - If you are submitting issue on any site that requires an account (cookies), a valid account mailed to the [org email address](lolipopplus@protonmail.com) may be necessary. By doing that you are trusting [org owner](https://github.com/Rictusempra) enough.
- Here are service inavailablity things that won't be fixed:
    -  from contents blocked by any built-in subscriptions
    -  caused by certain preferences outside of rule sets or of uMatrix itself
    -  if a site:
        -  is using SSL cert from any untrusted CA
        -  containing **mostly only** pornographic content
        -  reported as a deceptive site
        -  is a private blog site that is not hosted on public serivce
    -  relevant with any plugin, such as Adobe Flash
    -  other issues you should have learnt from uMatrix [README](https://github.com/gorhill/uMatrix/blob/master/README.md) or [wiki](https://github.com/gorhill/uMatrix/wiki)

---

### Reeshoova! - 许可协议

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
除非额外声明，否则本组织中全部内容许可协议均为 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
