## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava---toc)

[uMatrix wiki](https://github.com/gorhill/uMatrix/wiki/Cookies)に言ったとおり、uMatrixはすべてのcookiesの`遺留を阻止すること`が出来ます。これらの指示に従うことをおすすめします
：

ルール追加 `* * cookie block`，サイトのすべてのcookiesを阻止する。この後マニュアルで特定のサイトにcookiesを起用することが必要とされます。例：

    * * cookie block
    google.com accounts.google.com cookie allow
    google.com google.com cookie block

この状況で，`google.com google.com cookie block`はGoogleサーチエンジンのcookiesトラッキングを阻止、同時に`google.com accounts.google.com cookie allow` はGoogleアカウントに関するサービスを保証する。このような実装は[ここ](https://github.com/uMatrix-Rules/uMatrix-Rules-Site/tree/Strict-Cookies)にあります。

### Reeshoova! - 使用許諾契約

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>テキストは <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>の下で利用可能です。追加の条件が適用される場合があります。