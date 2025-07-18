## 自動販売機（オブジェクト、DOM、イベント処理）のミニレポート
### Q4-1. Itemクラスのメソッドについて説明せよ。
* showItemListがクラスメソッドである理由を考察せよ。:商品の一覧表示は特定のインスタンスに依存しないため、クラス全体で使えるクラスメソッドにしている。
* buyItemがインスタンスメソッドである理由を考察せよ。:購入処理は各商品ごとの在庫を減らすため、個々のインスタンスに対して行う必要があるから。
### Q4-2. 商品の購入ボタンをクリックすると、どのような処理でセルの値が減少するか説明せよ。
* 購入された商品の在庫数のセルをどのようにして特定するのか説明せよ。:各商品の在庫数セルには、商品IDを含むID属性（例：'stock1'）が割り当てられており、'document.getElementById("stock" + 商品ID)' で在庫数のセルを特定します。
* 特定したセルの値をどのように変更するのか説明せよ。:セルのテキスト内容を更新するために、DOM要素の'textContent'または'innerText'プロパティに新しい在庫数をセットし、画面表示を反映させます。
### Q4-3. 感想
* 今回の課題で苦労したこと: 購入ボタンのクリックイベントに適切に商品ごとのメソッドを紐付ける処理などを正しく実装するのに苦労しました。
* 演習を通して理解できたこと:JavaScriptのクラス構文の使い方、インスタンスとクラスメソッドの違い、DOM操作とイベント処理の連携が具体的に理解できました。
* この自動販売機プログラムの追加機能や課題など:商品の補充機能や売り切れ時の購入ボタンの無効化。
