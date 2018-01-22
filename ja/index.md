## Vrooboo! Wabbo!!

ここはuMatrixの規則と使用説明の詰め場所です。

[uMatrix](https://github.com/gorhill/uMatrix) はブラウザ拡張機能、ネットワーク要求のソース、タイプ、宛先などに基づいてポイントベースの制御を行うことができます。

---

## Ovagarava - T.O.C.

- [ブラックリストモード](Blacklist-Mode.md)
- [ガイドライン](Guidelines.md)
- [クッキーコントロール](Cookies-Control.md)
- [uMatrix と uBlock Origin の区別](Differences.md)
- [臨時規則](Temp.md)
- サードパーティフレームワーク    
    - [Googleサービス](Google-Services.md)
    - [ビデオIframe（例）](Video-Iframe-Examples.md)
    - [他のサードパーティフレームワーク](Others.md)
- [uMatrix ボタン功能の説明](Visual.md)

---

## Shagdovala - FAQs

1. サードパーティ要素許可の基礎は？

    一番大事なのは日常的に使用されるほぼすべてのサイトが正常に機能すること。機能を確保した上、ブロックされた要素の数を最大限にすること。

2. uMatrixだけで十分ですが？他のプライバシー増強ツールありますが？

    勿論uMatrixだけでは不十分です。一部のサードパーティ要素には、通常のサイト機能とトラッキングスクリプトの両方が含まれています。これらのツールが役に立つかもしれない：
    
    - [CanvasBlocker](https://github.com/kkapsner/CanvasBlocker)：簡単なプロテクターツール    
    - [Cookie-AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete)：`アクティブモード`には慎重に
    - [Decentraleyes](https://decentraleyes.org/)：おすすめです！    
    - [Don't Fuck With Paste](https://addons.mozilla.org/firefox/addon/don-t-fuck-with-paste/)：特定のウェブサイトの機能を破壊する可能性あり
    - [HTTPS Everywhere](https://www.eff.org/https-everywhere)：RAMを大量使用の上に、機能に重大な問題があります。
    - [Neat URL](http://hugsmile.eu/)
    - [NoProfile](https://addons.mozilla.org/firefox/addon/noprofile/)：一部のサイト、特にマウスオーバー効果が非常に多い場合には動作が異常になることがあります。   
    - [uBlock Origin](https://github.com/gorhill/uBlock)：おすすめのコンビネーション
    - [URL Tooltip WE](https://addons.mozilla.org/firefox/addon/url-tooltip-we/)

    もし[Mozilla Firefox](https://www.mozilla.org/firefox/all/)を使用した場合、バッテリーAPIが追跡されるのを避けるために削除されているにもかかわらず、これらの指示に従うことがおすすめです：

    - `about:preferences#privacy`
        - `履歴`のFirefox に`履歴を一切記憶させない`を選択。 
        - `トラッキング保護`の二つの`常に`を選択 。
        - `許可設定`の`アクセシビリティサービスによるブラウザーへのアクセスを止める`を選択。
        -`セキュリティ`の`危険な詐欺コンテンツをブロックする`を**選択しない**：この機能は Google Safe Browsing API を使用している、そして常にユーザーを追跡します。もし必要があるのならプロフェショナルのアンチウイルスソフトウェアを使用してください。
    - `about:preferences#search`
        - `既定の検索エンジン`の`アドレスバーに検索候補を表示する`を**選択しない**：これによって検索エンジンは情報を収集することができます。必要があれば、代わりに検索を記録しないエンジンDuckDuckGoを使用することがお勧めします。　

3. 寄付する方法は？

    [私たちは](https://github.com/Rictusempra)寄付を受け取るつもりはありません。[他のメンバー](https://github.com/orgs/uMatrix-Rules/people)に寄付のことを確認してください。

4. このウェブサイトの奇妙な言葉の意味は？

    これらの言葉はMMORPG`League Of Legends`のキャラクター`ナール`のセリフです。[こちらに](http://leagueoflegends.wikia.com/wiki/Gnar/Quotes)他のセリフを確認してください！

## Gnar gada! - 使用方法　

1. まずは適切な規則を選択してください：：[domain](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain) あるいは [site](https://github.com/uMatrix-Rules/uMatrix-Rules-Site)。後者がおすすめです。次に、`rules.txt`ファイルをローカルに保存するか、ブラウザに直接開いて内容全体をコピーしでください。
2. uMatrixダッシュボードを開いてください。
3. `自分のルール`タブに移動してください。　
4. ルールをインポート：
   -　`ファイルからインポートする`を選択し、先程ローカルに保存したファイルを選択してください。あるいは：
   - `編集` を選択し、クリップボードから貼り付けてください。5. `保存`してください。

## Shubbanuffa - 注意事項　
1. 一部のウェブサイトの機能が異常することがあります。自分責任で使用してください。
2. もし私たちに特定のサイトの問題を調査したいときは、[ここに](https://github.com/uMatrix-Rules)新しいissueを開いてください：
    - 具体的なURLを提供してください。
    - uMatrixとウェブブラウザーのversionも提供してください。
    - 自分が作ったルールとすべでのデフォルト設定に関する変更を提供してください。    
    - もしそのウェブサイトにアカウントが必要なばい、まずは使用することができるのアカウントを一つ[ここに](lolipopplus@protonmail.com)提出してください。それを送信されたばい、あなたがすべての[開発者](https://github.com/Rictusempra)に信頼することとします。
3. これらの状況に起こる異常事態には処理しません：
    -  サイト機能のコンテンツが組み込みサブスクリプションによってブロックされた
    -  サイト機能異常の原因はuMatrixルールの影響ではない
    - ウェブサイトがこれらの状況に適用される時：
        -  信頼できないCAによって発行された証明書を使用している
        -  **ほぼすべて**の内容はエロに関するもの
        -  危険なサイトとして報告された
        -  公共サービスでホストされていない個人的なブログサイト
    -  他の拡張機能、例えばAdobe Flash、に関する問題
    -  他にuMatrix [README](https://github.com/gorhill/uMatrix/blob/master/README.md)あるいは[wiki](https://github.com/gorhill/uMatrix/wiki)に提示された問題

---

### Reeshoova! - 使用許諾契約

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>テキストは <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>の下で利用可能です。追加の条件が適用される場合があります。
