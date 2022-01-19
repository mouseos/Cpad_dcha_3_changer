# Cpad\_dcha\_3\_changer

書きかけです。

必要なもの

*   チャレンジパッドNEO(それ以前の機種はもっと楽に改造できます。自分で調べてください。)
*   Windows,Linux,Mac OS搭載のPC(FreeBSDではできるかわかりません。)
*   USB Type B Miniケーブル

準備

１，Charlesを以下のURLからインストールします。

[https://www.charlesproxy.com/download/](https://www.charlesproxy.com/download/)

無料版と有料版がありますが無料版で問題ありません。

２，初期化済みチャレンジパッドNEOの電源を入れ、PCと同じwi-fiに接続します。

３，チャレンジパッドのipアドレスを調べます。設定アプリを開き、以下のように開きます。

設定→Wi-Fi→Wi-Fi設定→詳細設定

そこにIPアドレスという項目があります。192.168.から始まる行をメモしておいてください。

例：192.168.11.30

使い方

１，まずPCでCharlesを開きます。

![](https://user-images.githubusercontent.com/46545607/150069973-a1caa0d8-ec52-4cd9-8139-6860caa39fdb.png)

２，Proxy→Proxy settingsを開き、画像のように設定します。

![](https://user-images.githubusercontent.com/46545607/150070449-2f8413de-e142-429e-886a-f1d40fd584da.png)

![](https://user-images.githubusercontent.com/46545607/150070448-0f03137a-52b5-4639-b78b-d48ae29ed0b5.png)

設定が終わったらOKを押します。

３，Tools→Access control settingsを開きます。

![](https://user-images.githubusercontent.com/46545607/150070951-0e2c40dc-e021-4ec9-8a11-9ff7a34e9c1c.png)

Addを押して先程調べたIPアドレスを入力します。ここでは192.168.11.30です。

入力後はOKを押します。

４，Proxy→SSL Proxying Settingsを開き、画像のように設定します。

![](https://user-images.githubusercontent.com/46545607/150072166-354e90b7-f560-4913-8af9-a7db4876e859.png)

設定後OKを押します。

５，Tools→Rewriteを開きます。

![](https://user-images.githubusercontent.com/46545607/150072490-991cc50a-9941-46b0-a795-0c2e254244e2.png)

６，Addを押してUntitled Setを追加後Untitled Setを選択します。

![](https://user-images.githubusercontent.com/46545607/150072831-16124fc9-641c-4610-9276-abaa24988852.png)

７，上の画像のような画面が出るので、上部のAddを押します。

![](https://user-images.githubusercontent.com/46545607/150072963-1fa59517-96c2-4eab-9ec3-3b216d343536.png)

上の画像のように設定します。設定値は次のとおりです。

Protocol: https

Host: townak.benesse.ne.jp

Port: 443

Path: rel/A/sp\_84/open/TouchSetupLogin.apk

Query: 空欄

設定後OKを押します。
