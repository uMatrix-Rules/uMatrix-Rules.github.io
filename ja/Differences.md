## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava---toc)あなたが疑問があるかもしれません：なぜuMatrixが必要でしょう、私は既にuBlock Originの

コンソールで、高度なユーザーモードを選択し、手動で永久ルール `* * 3p block` 、`* * 3p-script block` 、`* * 3p-frame block` を増加しましたよ？これらのルールによって、あなたがuBlock Originの

[ハードモード](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode)を起動しました。

一般に、uMatrixは`要素制御`に重点を置いており、uBlock Originは`ドメイン制御`と`精細要求フィルタリング`機能をよりよく処理します。具体的には：

#### 要素制御任意のYouTubeの動画再生ページで，uMatrixまたはuBlock Origin

[ハードモード](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode)のいずれかを開くと、コメント領域の下部がブロックされます。コメント領域を復元する方法は次のとおりです：

-  uBlock Originツールバーのポップアップウィンドウを開き，`google.com` がらの任意のタイプのページリクエストを許可するをクリックしてください。在此情况下， この場合、google.comがら**任意のタイプ**のページリクエストが許可されます。
- uMatrixツールバーのポップアップを開き、`脚本` と `cookie`のページリクエスト許可します。したがって、google.comからの他のタイプのページリクエストは**ブロッキングを維持します**。この二つの方法のいずれにせよ、YouTubeのコメント領域が回復することができます。しかし、明らかにuMatrixはより効果的な要素制御機能を持っている。

#### 精細要求フィルタリング

uBlock Originには、多数の組み込みルールサブスクリプションがあり、すべてのAdBlock Plus構文と互換性があります。 その逆、UMatrixは、細かいフィルタリングに不十分があります。先程の例により

，uMatrixを使用すると`google.com`から**すべて**のスクリプトを許可またはブロックすることしかできません。 しかし、uBlock Originは任意の数のスクリプトをブロックすることができます。その方法は簡単、uBlock Originコンソールの`Custom Rules`タブでルールを作成するか、または[Element-picker](https://github.com/gorhill/uBlock/wiki/Element-picker)あるいは他のビルトインツールを使用すると簡単にできます。

### Reeshoova! - 使用許諾契約<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
テキストは <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
の下で利用可能です。追加の条件が適用される場合があります。