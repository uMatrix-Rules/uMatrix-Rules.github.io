## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava)

You may wonder the why uMatrix is still necessary even if you have checked `I am an advanced user` on uBlock Origin's dashboard and added `* * 3p block`, `* * 3p-script block`, `* * 3p-frame block`as permanent custom rules toward uBlock Origin.

By applying with those preferences, you are toggling [Hard Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode) of uBlock Origin.

uMatrix concentrates on, conclusively, `elements control` while uBlock Origin handles `domain control` & `precise request filtering`. This explains as:

#### Elements Control

On any video playing page on YouTube, you will find YouTube comment area is block by both uMatrix or uBlock Origin [Hard Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode). To restore the facility, you shall:

- on uBlock Origin toolbar button's popping up, click & allow web requests from `goole.com`. In this case, **any type** of web requests from `goole.com` is allowed.
- on uMatrix, click & allow both `cookie` & `script` from `google.com`. This will **keep blocking** any other types of elements from `google.com`.

In both way, you will be able to use comment area on YouTube again. But clearly uMatrix has more ability on `elements control`.

#### Precise Request Filtering

uBlock Origin has a trunk of built-in rules subscriptions and is compatible with rules under all types of AdBlock Plus syntax. uMatrix has, clearly, poor ability on this.

Take the previous case as an example, you can only allow or block all scripts from `goole.com` with uMatrix. But uBlock Origin allows you block any number of them. To achieve that, simply create a custom rule on `My Rules` tab on uBlock Origin's dashboard or utilize [element picker](https://github.com/gorhill/uBlock/wiki/Element-picker) or any other convenient built-in tools.

### Reeshoova!

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
Except where otherwise noted, all content in this org is licensed under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>