ChangeLog
=========

4.0.0 (2026/10/22)
--------------------
### 💥BREAKING CHANGES
- Drop Node.js v16.x, v18.x support
- Now support Node.js version is 22 or later

### To Update
以下を実施してください
- Dockerfile 確認 (Alpine Linux v3.18 -> v3.22, Node.js v18.20.1 -> v24.22)
- Areionskey 再起動

### ✨Improvements
- Based on mei-v11 [11.37.1-20240721044611](https://github.com/mei23/misskey-v11/releases/tag/11.37.1-20240721044611)

### 🐛Fixes
- mention: `@twitter.com` でのリンク先を修正
- 依存関係の更新

3.1.1 (2024/04/06)
--------------------
### To Update
以下を実施してください
- Dockerfile 確認 (Node.js v18.17.1 -> v18.20.1)
- Areionskey 再起動

### 🐛Fixes
- 依存関係の更新

3.1.0 (2023/11/29)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- Server/AP: signed headers の認証 by @mei23, @perillamint, @yunochi, @zotanmew [d4710e6](https://github.com/sakura-tel/areionskey/commit/d4710e63e3738350cba4e3f145dba783d779fede)
- Package: migration:revert を呼べるように by @mei23 [8f71cf3](https://github.com/sakura-tel/areionskey/commit/8f71cf31bfeb4614fcd2728adfc31c466219f09a)
- node-fetch -> got に完全移行 by @mei23 [491c29f](https://github.com/sakura-tel/areionskey/commit/491c29f1bdf1d37a794cc520853c27ed4879a335)
- Note/Polls: ローカルのみの note では Update を配信しないように bt @mei23 [c3e289d](https://github.com/sakura-tel/areionskey/commit/c3e289d283af6571eab1e1f639258d939256fef2)
- Note: 編集を受信可能に by @mei23 [0832337](https://github.com/sakura-tel/areionskey/commit/08323374ea96fcb2d3819684bfdda40099e09ffc)
- Note: 検索可能性を追加 by @mei23 [d8c8ddb](https://github.com/sakura-tel/areionskey/commit/d8c8ddbe74c1e283a0cbd85b7f4de88eeadd82e3) [fd0b903](https://github.com/sakura-tel/areionskey/commit/fd0b90364e1493c451f019bce1db481ff4848686)
- Server/Web: DNS Lookup に CacheableLookup を利用するように by @mei23 [00f1864](https://github.com/sakura-tel/areionskey/commit/8f02f5c92638e398da6d13d4a9e21b16d1531938)
- Note: 組み込み動画プレーヤー by @mei23 [6401793](https://github.com/sakura-tel/areionskey/commit/6401793268c02bc3d7eb32503dff2ab6b71ff33f)
- CSP by @mei23 [8bc1a5d](https://github.com/sakura-tel/areionskey/commit/8bc1a5ded6ffee4e672b8d6baadfa680517ea388)
- Note: プレビュー(サマリ)の改善 by @mei23 [46d8b56](https://github.com/sakura-tel/areionskey/commit/46d8b567462f995a3c77f3a7e9562c23f3cffbdc) [a9ef440](https://github.com/sakura-tel/areionskey/commit/a9ef440d01fa38c62202700cb7d74430d4a84c95) 
- Test: URL チェックの改善 by @mei23 [5cfd288](https://github.com/sakura-tel/areionskey/commit/5cfd288fef854672cdea65b03e306614699b14d4)
- Link: Discord ユーザ名規則の変更 by @mei23 [9a10726](https://github.com/sakura-tel/areionskey/commit/9a10726f8485046633d7fe2b21d2a1eea8347945)

### 🐛Fixes
- Emoji: List 修正 by @mei23 [dcddba0](https://github.com/sakura-tel/areionskey/commit/dcddba00033a613cf4fd484fb955471504ebc43c)
- api-doc: Chrome から閲覧できるように修正 by @mei23 [1670be1](https://github.com/sakura-tel/areionskey/commit/1670be103f3efe9060a0f05d3e2f7c222a0bfdf9)
- Server: Queue 制限のチューン by @mei23 [4c8316e](https://github.com/sakura-tel/areionskey/commit/4c8316e278af87f578e4dfe497afae11fce2452f)
- ルームを利用できるように修正 by @fs5m8 [00f1864](https://github.com/sakura-tel/areionskey/commit/00f1864d840d86d65fc7f838a14cbb833e2624ae)
- 言語ファイルの更新
- 依存関係の更新

### Put on hold
- Test: 項目に HTML meta を追加 by @mei23 [5bb35ec](https://github.com/sakura-tel/areionskey/commit/5bb35ecb5d470353f95adb3f48bc01c8db382fa3)

3.0.0 (2023/08/17)
--------------------
### 💥BREAKING CHANGES
- Drop Node.js v14.x support
- Now support Node.js version is 16.20.1 or later

### To Update
以下を実施してください
- Dockerfile 確認 (Alpine Linux v3.15 -> v3.18, Node.js v18.12.1 -> v18.17.1 )
- Areionskey 再起動

### ✨Improvements
- Search: ユーザネームによる検索を改善 by @fs5m8 [e2201a0](https://github.com/sakura-tel/areionskey/commit/e2201a02fc7649276586d1a75b602c7fa6deb5c7)
- Endpoint: ユーザネームやホストで検索可能に by @sousuke0422 [96d7925](https://github.com/sakura-tel/areionskey/commit/96d7925b1ab67eaa829daeac72fde3fb033a907f)
- Export: ファイルをURLを含めるように変更 by @CGsama [a820b7d](https://github.com/sakura-tel/areionskey/commit/a820b7d3ffefbd7907a92d339f91d9c6bbc4d46c)
- Reaction: 作成時のパフォーマンスを改善 by @mei23 [90abd62](https://github.com/sakura-tel/areionskey/commit/90abd62fcd4c17c80789baa4e9c2cda4a3a41ebc)

### 🐛Fixes
- 2FA: 有効にすると必ずサインイン時にサインインできないのを修正 by @fs5m8 [c33b233](https://github.com/sakura-tel/areionskey/commit/c33b2339145ceb95e1ed6ad42466879cc9d4ccf4)
- 言語ファイルの更新
- 依存関係の更新

2.4.3 (2023/05/14)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- Emoji-picker: サイズ等変更 by @fs5m8 [83117ac](https://github.com/sakura-tel/areionskey/commit/83117acea54b9096bbb89c1479c00474aa54107a) [9fa797a](https://github.com/sakura-tel/areionskey/commit/9fa797a23fcbf7ffc581c1d09740f106baadd62a)
- Emoji-picker: Skintones に対応 by @mei23 [281d11d](https://github.com/sakura-tel/areionskey/commit/281d11dd6b10dd0a236408563aa1906cec622ed6)
- Admin: 公式・プレミアム・Cat・Bot アカウント を表示するように by @atsu1125 [5b53fc1](https://github.com/sakura-tel/areionskey/commit/5b53fc15204aec032a439dce021d1798a67e2091)
- User: アカウントの見つけやすさを追加 by @atsu1125 [21f3bec](https://github.com/sakura-tel/areionskey/commit/21f3bec2d03e7b27e7ebd29d39ff2427f3d40397)
- URLチェックの強化 by @mei23 [3619cec](https://github.com/sakura-tel/areionskey/commit/3619cec0405b483572156d3dea21f05e8c02ab2d)

### 🐛Fixes
- Deck: デッキを読む際にタイムラインを2回ロードしてしまうのを修正 by @mei23 [18d6d16](https://github.com/sakura-tel/areionskey/commit/18d6d1669262a5325fc5508bf59fecb4cc365720)
- 依存関係の更新

### ❌Abolitions
- DB: log を削除 by @fs5m8 [4cb73bb](https://github.com/sakura-tel/areionskey/commit/4cb73bb7b810aa8ea848748d99ef65420f0c26fa)

2.4.2 (2023/02/11)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- OGP: 項目を追加 by @fs5m8 [2d35b67](https://github.com/sakura-tel/areionskey/commit/2d35b67cec463b90f576f7e6dd62f1c574f17f35)
- URLチェックの強化 by @mei23 [cd43d69](https://github.com/sakura-tel/areionskey/commit/cd43d6943211e0ce5e49cf67f6cc4713f6cf21d1) [1f6ae07](https://github.com/sakura-tel/areionskey/commit/1f6ae07f57787ac2d24097847cc5cbaf263841f5) [88d237a](https://github.com/sakura-tel/areionskey/commit/88d237a18ae0fdd0e79b09929fa61542cf86e24b) [8f793fc](https://github.com/sakura-tel/areionskey/commit/8f793fc0f9ada1ab8412295ab5fcd64d14e90b61)
- admin: ファイル全削除の権限を変更 by @atsu1125 [827cf4b](https://github.com/sakura-tel/areionskey/commit/827cf4baeabbb7752db11ffb8fcf3100c7c5d42b)

### 🐛Fixes
- StyleSheet: 特定の固定幅フォントの指定を削除 by @fs5m8 [0a24cd7](https://github.com/sakura-tel/areionskey/commit/0a24cd728b8b7523aa35d9172500713abc6c30f7)
- 依存関係の更新

2.4.1 (2023/01/15)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- Unicode Emoji 15.0 by @mei23, @archaeme, @Johann150, @mia-0 [2a1ca22](https://github.com/sakura-tel/areionskey/commit/2a1ca22202159cfd6cee3d9090ee06b12fced243)
- diskusage -> check-disk-space by @mei23 [97a340b](https://github.com/sakura-tel/areionskey/commit/97a340b10dc8ce89ac53581dc32a56fba3fbc02b) [0b3d965](https://github.com/sakura-tel/areionskey/commit/0b3d9657a6076d00b06a3ff606e594b842d207ec)

### 🐛Fixes
- Depend: 本来ないといけない依存関係を追加など by @mei23 [374cb69](https://github.com/sakura-tel/areionskey/commit/374cb6910cdf73111dc0d7614a166f67ae910520)
- mobile: トーストの位置を修正 by @fs5m8 [7844e93](https://github.com/sakura-tel/areionskey/commit/7844e934d26de4262a79d9f5ce02ad784eb111de)
- reaction: カウントの文字の大きさを修正 by @fs5m8 [d3dda02](https://github.com/sakura-tel/areionskey/commit/d3dda02e81f9928b48444683cb8a7a209c8fb464)
- api/ep/emoji: カスタム絵文字名の重複チェックの修正 by @fs5m8 [bdc809c](https://github.com/sakura-tel/areionskey/commit/bdc809c659d1e0627c2339361455119cfa931266)

2.4.0 (2023/01/14)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- welcome/timeline: CW ボタンを追加 by @fs5m8 [8b191a5](https://github.com/sakura-tel/areionskey/commit/8b191a5e24960789f4cbb7921b53b9572032b90d)
- pages/aiscript: 変数を指す表記を `{ }` から `${ }` に変更 by @fs5m8 [078250d](https://github.com/sakura-tel/areionskey/commit/078250d681738295d6395d68814ef1a72c0bdc60) [ac96df6](https://github.com/sakura-tel/areionskey/commit/ac96df65ea8665e41bad21f21c2593a31e3c874e)
- service/drive: 不要なら画像のリサイズをしない 大きいJPEGの圧縮にMozjpegを使用するように変更 by @mei23 [5c67f61](https://github.com/sakura-tel/areionskey/commit/5c67f61ab6b8658abc39f15abe89e35b9c5649d8)
- mfm: strike の内部名を delete に変更 by @fs5m8 [ba0c188](https://github.com/sakura-tel/areionskey/commit/ba0c188831e4d4e8fd1e773413ac57b042b70006)
- mfm: カスタム絵文字の直前に カスタム絵文字名に含めることができる文字があるとき カスタム絵文字扱いをやめるように変更 by @fs5m8 [4de9dfa](https://github.com/sakura-tel/areionskey/commit/4de9dfa86a32c4f0440ba3c0f5e4049d7930ebd6) [eb54290](https://github.com/sakura-tel/areionskey/commit/eb542904fe756b5435eb0c9d020c7ad45edd0ddc) [3027922](https://github.com/sakura-tel/areionskey/commit/30279228fb6bb22d1ded738f427b1c848d779c73)
- api/ep/emoji: カスタム絵文字名の重複と不正な形式をチェックする処理を追加 by @fs5m8 [aae02be](https://github.com/sakura-tel/areionskey/commit/aae02be2644be42275c314ac48c1470bb1ac4a10)
- icon: unlock -> lock by @fs5m8 [9f30ed8](https://github.com/sakura-tel/areionskey/commit/9f30ed8d5f31c4feb2dbdbb4aa5aa131e76a0bd2)
- postform: 引用として投稿される条件のときは Renote ではなく 引用 と表示するように変更 by @fs5m8 [458f978](https://github.com/sakura-tel/areionskey/commit/458f9787ddd83f883ecd79cab778ca75fff8a82d)
- Dev: backend の build に swc を使用するように変更 by @mei23 [842f6bb](https://github.com/sakura-tel/areionskey/commit/842f6bb3e96c34ca5a9f749c885b95a16dbbbd94) [837246e](https://github.com/sakura-tel/areionskey/commit/837246efab2cfd6707e0c9a788f8f87da60352e1)
- Dev: webpack.config を js に変更 by @mei23 [186fdab](https://github.com/sakura-tel/areionskey/commit/186fdab77ef84bd70cd843ca57e0a3864cf62762)
- Dev: gulpfile を js に変更 by @mei23 [7ae458b](https://github.com/sakura-tel/areionskey/commit/7ae458b71424942e7e5c5e3d5be7bb441d46b9b9)
- Dev: TypeScript の Linter に ESLint を使用 by @mei23 [7dced81](https://github.com/sakura-tel/areionskey/commit/7dced8139b348deac7e625b8efe3871993d2b80f)
- user: ブロックしているときはフォローボタンを非表示にする変更 by @atsu1125 [4cd05ed](https://github.com/sakura-tel/areionskey/commit/4cd05ed218a1638a5d414187f56cc2ee0a9eb2b2)

### 🐛Fixes
- desktop/header/menu: アイコンの並びを統一 by @fs5m8 [43adf82](https://github.com/sakura-tel/areionskey/commit/43adf8252f040901f195343483ef076ffcdef424)
- drive/files: 形式バリデータの修正 by @mei23 [ea2bc3f](https://github.com/sakura-tel/areionskey/commit/ea2bc3fefff445520a02565344f1e8dc94cd306c)
- SQL LIKE escape by @mei23 [22f9ea5](https://github.com/sakura-tel/areionskey/commit/22f9ea50e199780c7808d6750d2446a4b686dce9)
- Dev: build に不要な依存パッケージを devDependencies に移動 by @mei23 [ce0bd05](https://github.com/sakura-tel/areionskey/commit/ce0bd05ef795033a2b5bdce963019604e79eb730)
- settings: API token を隠すように変更 by @atsu1125 [7e0d6a4](https://github.com/sakura-tel/areionskey/commit/7e0d6a4a4870aa33adfb5a6ab94f176c5e3d8e44)
- その他 `mergin`, `padding`, `overflow` などの調整
- 言語ファイルの更新
- 依存関係，テストファイルの更新

### ❌Abolitions
- mfm: `big` の動きを削除 by @fs5m8 [9ecb280](https://github.com/sakura-tel/areionskey/commit/9ecb280e17ba87f58e209e53f5213a238c3cad85)
- mfm: `motion`, `jump`, `spin` の削除 by @fs5m8 [9ecb280](https://github.com/sakura-tel/areionskey/commit/9ecb280e17ba87f58e209e53f5213a238c3cad85)
- mfm: `title` の削除 by @fs5m8 [5e39c0d](https://github.com/sakura-tel/areionskey/commit/5e39c0d5715dd1e169e9358b17aacbc5399d23c8)

2.3.0 (2023/01/04)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

`docker-compose.yml` の PostgreSQL デフォルトバージョンを `11.2` から `15.x` に，Redis デフォルトバージョンを `4.0.x` から `6.2.x` に変更しました．付属の `docker-compose.yml` で直接実行している場合は，環境に合わせて 書き換え または アップデートを実施してください．

### ✨Improvements
- reaction: 絵文字の下に影を追加 by @fs5m8 [518e5b2](https://github.com/sakura-tel/areionskey/commit/518e5b209457e5c3919c086746faf35697a90a6a)
- emoji-picker: 画像を遅延読込に変更 by @fs5m8 [957b72c](https://github.com/sakura-tel/areionskey/commit/957b72ca43f2e463ee25fe737c4f85b5a8cd422e)
- mobile/reaction: マウスオーバ時の表示を Mobile でも表示するように変更 by @fs5m8 [f6491f0](https://github.com/sakura-tel/areionskey/commit/f6491f0a0390593d5b3928360536995edbdfddbf)
- emoji: sticker (スタンプ) 機能を追加 by @EbiseLutica mod @fs5m8 [4a2f225](https://github.com/sakura-tel/areionskey/commit/4a2f225a2ab65d401f5b83874c403f22954b3561)
- emoji: カスタム絵文字は大きく表示するか否かを選択可能に変更 by @EbiseLutica mod @fs5m8 [5fa1db5](https://github.com/sakura-tel/areionskey/commit/5fa1db55c17eee2c59933aa1b08ba0535555da3a)
- reaction: マウスオーバ時の表示を Misskey v12 相当の表示に変更 by @fs5m8 [203a4e6](https://github.com/sakura-tel/areionskey/commit/203a4e6d63f08f9fb03fcb01e3ef06fe17245035)
- user: モデレータのバッジを追加 by @atsu1125 [7498f77](https://github.com/sakura-tel/areionskey/commit/7498f775f1e7a8409d4e2cc2dbd41aa5497e9fb3)
- admin: メニュー内の自分の名前の下に役割を追加 by @atsu1125 [ed80968](https://github.com/sakura-tel/areionskey/commit/ed8096850a24cb5861b9172fa0ae9a6aa59c16b6)
- emoji-picker: 検索機能を追加 by @sousuke0422 [4646c03](https://github.com/sakura-tel/areionskey/commit/4646c03d81df5270c1002b8c107ccf317295a284) [283925a](https://github.com/sakura-tel/areionskey/commit/283925a5529d057a1216e0e4e54571e614cd38c3)
- reaction-picker: 絵文字ピッカーを追加 by @sousuke0422 [50f5f24](https://github.com/sakura-tel/areionskey/commit/50f5f246fb9744cffc2da32630ec5b84af54b685)

### 🐛Fixes
- desktop/crop: ボタン類のフォーマットを他のウインドウと統一するように変更 by @fs5m8 [67a1a4e](https://github.com/sakura-tel/areionskey/commit/67a1a4ead35d7be7db178136033e047d751da18a) [67a1a4e](https://github.com/sakura-tel/areionskey/commit/67a1a4e9a8a48eefec0e62016e2d449eddafa459)
- 参照置換 `api/admin/show-user` -> `api/users/show` by @fs5m8 [dbbe3f6](https://github.com/sakura-tel/areionskey/commit/dbbe3f6f3526c28bd2e71d38d00f88dd4bf42f70)
- avatar/cat: ネコミミをアバター画像の平均色となるように変更 by @fs5m8 [cd97f08](https://github.com/sakura-tel/areionskey/commit/cd97f085fd230b13764422c3935b7ed6d06c699b)
- autocomplete: 画像を中央揃えに変更 by @fs5m8 [8be6e0d](https://github.com/sakura-tel/areionskey/commit/8be6e0d2b94b4a5bb9c20c49e24778d8c0862826)
- report: `admin` を通報可能に変更 by @atsu1125 [85e5ff8](https://github.com/sakura-tel/areionskey/commit/85e5ff8468cc8343858d0339f936eb0d6eb1ffec)
- note: リアクション数合計をタイムラインではなく 当該の投稿の詳細画面に表示するように変更 by @fs5m8 [5965173](https://github.com/sakura-tel/areionskey/commit/59651739174cef7463d0f88e130d07fd2676c852)
- explore: 検索結果に「もっと表示」を表示しないように変更 by @fs5m8 [73905c7](https://github.com/sakura-tel/areionskey/commit/73905c70b11e4999899b5d565deb3d4cf3242022)
- desktop/header: サインアウト時はゲームを表示しないよう変更 by @fs5m8 [8082e1d](https://github.com/sakura-tel/areionskey/commit/8082e1d31fab7b9971fa8c995203b1d2503927de)
- mobile/emoji-picker: 出現する位置を調整 by @fs5m8 [0e0dec7](https://github.com/sakura-tel/areionskey/commit/0e0dec7a158b5981d327da64d6445f08aa0956ed)
- CSS: `backdrop-filter` を削除 by @fs5m8 [a6f9120](https://github.com/sakura-tel/areionskey/commit/a6f912027aa4f07c82f9b27c794714e1a526b472)
- admin: `moderator` の権限に合わせた frontend の調整 by @atsu1125 [6fb511d](https://github.com/sakura-tel/areionskey/commit/6fb511da083fe0170bd51b63e40d192ef9013926) [3ca49f3](https://github.com/sakura-tel/areionskey/commit/3ca49f3580480ad4eabd4e6ee2edbd6e46efef6e) [4a9c814](https://github.com/sakura-tel/areionskey/commit/4a9c814289c4c1645a736e9e06942a41c3d66144) [77751a0](https://github.com/sakura-tel/areionskey/commit/77751a0d91461961aa88c342778faba2f6fb397e)
- その他 `overflow`, `transparency` などの調整
- 言語ファイルの更新
- 依存関係，ワークフローファイル，テストファイルの更新

2.2.0 (2022/12/31)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- server: クライアントIPアドレスの取得元ヘッダを変更できるように変更 by @mei23 [88b8c0f](https://github.com/sakura-tel/areionskey/commit/88b8c0fa2f3462accbade30335f2440b2069977a)
- admin: 管理者によるアカウントの削除機能の追加 by @atsu1125 [PR#1066](https://github.com/sakura-tel/areionskey/pull/1066) [025673e](https://github.com/sakura-tel/areionskey/commit/025673e87fc1bb3b3c6e27d94d2602d1e2f9b9fc)
- admin/logs: 操作時にダイアログを表示するように変更 by @fs5m8 [025673e](https://github.com/sakura-tel/areionskey/commit/025673efcc3940dac64a8c7b6f068d65c2a0bf79)
- admin/db: 操作時にダイアログを表示するように変更 by @fs5m8 [a695887](https://github.com/sakura-tel/areionskey/commit/a695887fcc3940dac64a8c7b6f068d65c2a0bf79)
- frontend: メニューからデスクトップ/モバイルの切替ができるように変更 by @atsu1125 [PR#1063](https://github.com/sakura-tel/areionskey/pull/1063) [a695887](https://github.com/sakura-tel/areionskey/commit/a695887bbb1e667c209684a9849097597cd2c561)
- sound: トークのウインドウを閉じていても着信時に音を鳴らすように変更 by @fs5m8 [0479521](https://github.com/sakura-tel/areionskey/commit/047952113bf5553003899462c5247d895dae21ca)
- mobile/sound: モバイルでもサウンドが機能するように変更 by @fs5m8 [cec0fb0](https://github.com/sakura-tel/areionskey/commit/cec0fb06c56d1219d08be17f5a5313edcfa4a0d5)
- postform: プレビュー機能を無効化できるように変更 by @fs5m8 [0eb1488](https://github.com/sakura-tel/areionskey/commit/0eb1488d733bb8c48f3d94777e7b24b22a7f45fa)
- settings: isCat/isBot の説明を追加 by @fs5m8 [35cb4ba](https://github.com/sakura-tel/areionskey/commit/35cb4baf52b51c72e654c9d51bde7a6011a97a0a)

### 🐛Fixes
- server: X-Forwarded-For から クライアントIPアドレスを取得時は 1つ目だけ再帰するように変更 by @mei23 [35cb4ba](https://github.com/sakura-tel/areionskey/commit/35cb4ba2f3462accbade30335f2440b2069977a)
- activitypub: signToActivityPubGet をデフォルトで有効に変更 by @mei23 [c94ecfd](https://github.com/sakura-tel/areionskey/commit/c94ecfd3a392e768b14e309422d423901a834347)
- server/inbox: inboxのサイズリミットを1MBから64KBに変更 by @mei23 [6e1d936](https://github.com/sakura-tel/areionskey/commit/6e1d936c6cea32cf969bda794e7d80a787ed5413)
- admin: 非ログイン時にアクセス拒否表示が表示されないのを修正 by @atsu1125 [PR#1062](https://github.com/sakura-tel/areionskey/pull/1062) [de078e7](https://github.com/sakura-tel/areionskey/commit/de078e7440b48211f8ab90de28b7f0fc11aa5d54)
- assets: 整理と音声の定位を中央に変更 by @fs5m8 [dd47191](https://github.com/sakura-tel/areionskey/commit/dd471915b0d2788ecd40a66e44acf4b7395d3fa7)
- mobile/widgets: テーマに適合するように変更 by @fs5m8 [c5bb452](https://github.com/sakura-tel/areionskey/commit/c5bb452c80348a6466e79db1772867dd0a89e8b2)
- mobile/user: テーマに適合するように変更 by @fs5m8 [c5bb452](https://github.com/sakura-tel/areionskey/commit/c5bb452c80348a6466e79db1772867dd0a89e8b2)
- mobile/drive/folder-chooser: テーマに適合するように変更 by @fs5m8 [c5bb452](https://github.com/sakura-tel/areionskey/commit/c5bb452c80348a6466e79db1772867dd0a89e8b2)
- desktop/header/clock: テーマに適合するように変更 by @fs5m8 [0b8a01e](https://github.com/sakura-tel/areionskey/commit/0b8a01e4b6dda6be88076c2f72e354a3daaf9ddf)
- mobile: focus 時のアウトラインを非表示に変更 by @fs5m8 [b6c2058](https://github.com/sakura-tel/areionskey/commit/b6c2058f79fd61dd9bdd518f66b902ca3ba5bcf3)
- mobile/postform: 最近のハッシュタグの表示が2つもあったので片方を削除 by @fs5m8 [a015b41](https://github.com/sakura-tel/areionskey/commit/a015b415a12bb53db767add1e417fc3fcb2c712b)
- TypeScript: String.substr() -> String.substring() by @fs5m8 [eb40267](https://github.com/sakura-tel/areionskey/commit/eb402679560d5d1219b46e8f70d6c61be6271481)
- CSS: 廃止された/不要になった CSS プロパティの削除 by @fs5m8 [8a37c22](https://github.com/sakura-tel/areionskey/commit/8a37c2248bf7dcbcc7fe24cca5ff16a3ad36f0e3)
- その他 mergin/padding の調整
- 言語ファイルや文書の更新
- 依存関係の更新

2.1.1 (2022/12/25)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- sound: 通知音を追加, サウンドの個別 ON/OFF 機能を追加 by @fs5m8 [56fba4c](https://github.com/sakura-tel/areionskey/commit/56fba4c559fa67e691a53e0686d8d51f27b2c7f6)

### 🐛Fixes
- image: サムネイルの余白は塗り潰すように変更 by @fs5m8 [7a97403](https://github.com/sakura-tel/areionskey/commit/7a974038748bc6cf8e5feb91a1ee5134d2098192)
- misc/fetch: 取得する JSON の大きさを 256kB に制限するよう変更 by @fs5m8 [9a5ced7](https://github.com/sakura-tel/areionskey/commit/9a5ced7f150461d775adf685ba3484ff941d04c3)
- block: ブロック時に RejectFollow するよう変更 by @mei23 (from Mei v11) [755fab1](https://github.com/sakura-tel/areionskey/commit/755fab1814ad8a405472085ca97d15db847e44d5)
- image: サムネイルの表示が cover になっていたのを修正 by @mei23 (from Mei v11) [a333f60](https://github.com/sakura-tel/areionskey/commit/a333f60fe57879ca3fbba4b1bdb7885e4b33e8a1)
- nav: フォローリクエストの項目を フォローリクエストがあるときのみ表示するよう変更 by @fs5m8 [0f5b05f](https://github.com/sakura-tel/areionskey/commit/0f5b05f494ddb329785ad103e7a2abf580752c29)
- configfiles: 投稿ID生成のデフォルトを ULID に変更 by @fs5m8 [167b032](https://github.com/sakura-tel/areionskey/commit/167b03226fa7574df2d59337d3cdb624cf01c2fd)
- admin: アクセス拒否時のテキストを 全体表示にし，i18n対応に変更 by @fs5m8 [fb68f6e](https://github.com/sakura-tel/areionskey/commit/fb68f6e3e29c7159edb301df70cc96ad9ff08584)
- login/out -> signin/out 語彙を変更 by @fs5m8 [b52b8de](https://github.com/sakura-tel/areionskey/commit/b52b8de8c0b959cde226a83b4163aa019efe411e)
- desktop/header: 開発ビルド警告バーの flush のリンク先を変更 by @fs5m8 [730f035](https://github.com/sakura-tel/areionskey/commit/730f035c0380b23f14dc6f16fa78ae9ae829614b)
- signin: 不要なメソッドを削除 by @fs5m8 [a2c2e98](https://github.com/sakura-tel/areionskey/commit/a2c2e989772c3a9f653ed0c1bcd736afe2a2a0dd)
- signin/flush: ダイアログをリッチに変更 by @fs5m8 [6d6b8f8](https://github.com/sakura-tel/areionskey/commit/6d6b8f87a3283cc4a4d682cc32b6d8571532459a)
- ui-container: ヘッダをクリックしても展開しないよう変更 by @fs5m8 [89b3e2d](https://github.com/sakura-tel/areionskey/commit/89b3e2d877db02748e54ae55ded3477ed66bd57d) 
- その他 font-size/mergin/padding の調整
- 統一されていない文言やアイコンを統一
- 言語ファイルや文書の更新
- 依存関係の更新

### ❌Abolitions
- note/menu: メンション 項目を削除 by @fs5m8 [09e2345](https://github.com/sakura-tel/areionskey/commit/09e2345349145486dda1b0aa82a9f1f89c6952c9)
- desktop/settings: アプリをメニューから削除 by @fs5m8 [5020614](https://github.com/sakura-tel/areionskey/commit/5020614817fad83e8d1bf97a1cf66a11d92876e4)
- widget: hashtag(trends) を削除 by @fs5m8 [caa864a](https://github.com/sakura-tel/areionskey/commit/caa864abd7fba89c47547329108d49cd45efe897)
- page: featured を削除 by @fs5m8 [caa864a](https://github.com/sakura-tel/areionskey/commit/caa864abd7fba89c47547329108d49cd45efe897)
- component: tag-cloud, trends を削除 by @fs5m8 [caa864a](https://github.com/sakura-tel/areionskey/commit/caa864abd7fba89c47547329108d49cd45efe897)

2.1.0 (2022/12/18)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

Dockerfiles での Node デフォルトバージョンが 18.9.0 から 18.12.1 になっています

### ✨Improvements
- mobile/postform: プレビューを追加 by @EbiseLutica(from Groundpolis v2) [9189144](https://github.com/sakura-tel/areionskey/commit/91891445c0860bf283beb868f71711fe728cc8bf)
- mobile: 下部ナビゲーションバーを追加 by @EbiseLutica(from Groundpolis v2) [db1af2a](https://github.com/sakura-tel/areionskey/commit/db1af2a0bfa5b7543825c1d4dc0c3044a8635d38)
- profile: 場所/誕生日の設定項目に警告を表示 by @atsu1125 [PR#1037](https://github.com/sakura-tel/areionskey/pull/1037) [8f16281](https://github.com/sakura-tel/areionskey/commit/8f162818435029e4f6b1a742ab66b34af39e2522)
- 検索エンジンによるインデックスを拒否する機能を追加 by @atsu1125 [PR#1033](https://github.com/sakura-tel/areionskey/pull/1033) [41f664b](https://github.com/sakura-tel/areionskey/commit/41f664bed978acfcbd4fde02513bafb163e0351a)
- postform: ダイレクト投稿を選択したときに警告を表示 [9986cee](https://github.com/sakura-tel/areionskey/commit/9986ceef8eb717c4b7d039347fc16ff0e2c34733)
- welcome/timeline: リアクションを表示 by @atsu1125 [PR#1021](https://github.com/sakura-tel/areionskey/pull/1021) [9986cee](https://github.com/sakura-tel/areionskey/commit/9986cee915f994b28f60c2d55e855658153cc3ef)

### 🐛Fixes
- admin: 管理者/モデレータ以外がアクセスしたときにアクセス拒否画面を出すように変更 by @EbiseLutica(from Groundpolis v2) [3556f9c](https://github.com/sakura-tel/areionskey/commit/3556f9cbcf4219f5fa8004e0b59db9906b4f7395)
- mobile/notify: 引用符にまで色がついていたのを修正 [4c18113](https://github.com/sakura-tel/areionskey/commit/4c181139f151156fc235bc91fe8b22836d21b47b)
- note/menu: ブックマークやウォッチの操作後にメニューが開けるように修正 [54ee840](https://github.com/sakura-tel/areionskey/commit/54ee8403d1f89235454f1f3028832280b2066068)
- mobile/widget: ウィジェットを削除できるように修正 [afe8c83](https://github.com/sakura-tel/areionskey/commit/afe8c835e1839dca7e954f8a3efd3484d339bc3d)
- daemon/server: hideServerInfo = true 時にエラーが返るのを修正 by @atsu1125 [PR#1022](https://github.com/sakura-tel/areionskey/pull/1022) [3f76d15](https://github.com/sakura-tel/areionskey/commit/3f76d15ab49a36000c0ec9f43af06fa6f010ccd6)
- note/react: 自分のノートにリアクションできるように変更 by @atsu1125 [PR#1021](https://github.com/sakura-tel/areionskey/pull/1021) [a8138e2](https://github.com/sakura-tel/areionskey/commit/a8138e24246dfe817c864a548bbcc9ae777bc17d)
- admin: テキストボックスによる設定項目でスペースのみの項目が保存できてしまうのを修正 by @mei23(from Mei v11) [8319033](https://github.com/sakura-tel/areionskey/commit/831903304e4ccd1925b0cb460c819d413090a83c)
- Home posts -> Unlisted posts [5779815](https://github.com/sakura-tel/areionskey/commit/5779815ff4a87c331f05ed808ea497869681994e)
- explore: 無限ループしないように修正 [bb11d3c](https://github.com/sakura-tel/areionskey/commit/bb11d3caae3f8bc572d8f0c891c959b2d2600886)
- widget/stickynote: 即時保存するように変更 [63dfef9](https://github.com/sakura-tel/areionskey/commit/63dfef96fadd0f3ef431a399faa6390b28c151fa)
- その他 mergin/padding の調整
- 統一されていない文言やアイコンを統一
- 言語ファイルや文書の更新
- 依存関係の更新

2.0.0 (2022/12/04)
--------------------
### 💥BREAKING CHANGES
- Drop Node.js v12.x support

### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- めいv11 [v11.37.1-20221204012750](https://github.com/mei23/misskey-v11/releases/tag/11.37.1-20221204012750) by @mei23 までの変更/修正を適用

### 🐛Fixes
- favorite -> bookmark [19a2cc1](https://github.com/sakura-tel/areionskey/commit/19a2cc10de12b659bec8e2a9cf6240bd98749b64) [3737abd](https://github.com/sakura-tel/areionskey/commit/3737abdf09fc706572ef946112379770893ed036)
- profile: Location, birthday の連合 を修正 [853afa6](https://github.com/sakura-tel/areionskey/commit/853afa6007d49c51dd4f8db775dfd119fdc8235b)
- 依存関係の更新

1.6.3 (2022/12/03)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- 手動でのリモート情報の更新をする機能 を追加 by @EbiseLutica, @atsu1125 [PR#994](https://github.com/sakura-tel/areionskey/pull/994) [4594b7b](https://github.com/sakura-tel/areionskey/commit/4594b7b5fa7fd9f601a2125c3ab228398d761f99)
- profile: Location, birthday の連合 を追加 by @atsu1125 [PR#992](https://github.com/sakura-tel/areionskey/pull/992) [aab6ed3](https://github.com/sakura-tel/areionskey/commit/aab6ed32798a1916134013cce68bd3fc1b5036a1) [2ac9f6f](https://github.com/sakura-tel/areionskey/commit/2ac9f6f9530a9f53b2a8cc828674a9810e53ab0d) [c4a638c](https://github.com/sakura-tel/areionskey/commit/c4a638c7448a0866abfa002e58af568b30f69a38)
- Renote 取り消し機能 を追加 by @EbiseLutica, @atsu1125 [PR#984](https://github.com/sakura-tel/areionskey/pull/984) [b7fc5a3](https://github.com/sakura-tel/areionskey/commit/b7fc5a31b56002b0e5f3545e896b255726dcc6a8) [1234aa5](https://github.com/sakura-tel/areionskey/commit/1234aa5d6e0681fc27e78339272b5433a7c51137)

### 🐛Fixes
- forkbomb 攻撃に対処するための修正 by @mei23 [04ac49a](https://github.com/sakura-tel/areionskey/commit/04ac49a32f67dde786294209bf610fa6d352329d)
- モバイル: 非ログイン時のWelcome画面の 新規登録 / ログイン リンクの隙間 を調整 by @atsu1125 [PE#993](https://github.com/sakura-tel/areionskey/pull/993) [24951cf](https://github.com/sakura-tel/areionskey/commit/24951cfe9671703c6b679cab15db2bdbeaff8389)
- Deck: ハッシュタグタイムライン追加のダイアログ を改良 by @atsu1125 [PR#983](https://github.com/sakura-tel/areionskey/pull/983) [38f4da1](https://github.com/sakura-tel/areionskey/commit/38f4da1a3ca3b861902a09b9d831388481b4137b) [51dc14e](https://github.com/sakura-tel/areionskey/commit/51dc14e4cd2fc824c1a5c890d937ef773869c52b)
- 画像の更新
- 依存関係の更新

### ❌Abolitions
- ブロックの連合 を削除 [ae2be09](https://github.com/sakura-tel/areionskey/commit/ae2be095651e83b295f2e1c870c0d52a1aaf24b5)

1.6.2 (2022/12/03)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

緊急のリリースなので Changelog はリリース後に書きます

1.6.1 (2022/11/17)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

### ✨Improvements
- ユーザページに バッジを追加 [562f7d2](https://github.com/sakura-tel/areionskey/commit/562f7d28b516828850bb91a0d2b1af042dfcd5e5)

### 🐛Fixes
- DNS キャッシュをしないように変更 by @atsu1125 [b0facdf](https://github.com/sakura-tel/areionskey/commit/b0facdf9c77b60329b808b675ee09ae6054d66fe)
- データのエクスポートができなくなっていたのを修正 [ebe32ce](https://github.com/sakura-tel/areionskey/commit/ebe32ce1e43406c7c4c51e23abc1ea4bcbf9545c)
- 「閉鎖されているとマーク」を「配信停止」に変更 [7590578](https://github.com/sakura-tel/areionskey/commit/75905784050d46aa9fcf0d7bd1ed2568830ba3f9)
- Admin バッジ を ノートヘッダから削除，Bot バッジ を 文字からアイコンに変更 [e75deda](https://github.com/sakura-tel/areionskey/commit/e75dedaae35aa45aa1b2ddc90ee3b87e9b45ebb8) [3a28f17](https://github.com/sakura-tel/areionskey/commit/3a28f1727b9dce255f410f0e9912c54e0ae257e6)
- モバイル: ログインダイアログの OK(わかった) ボタンを削除 [1fcfcc8](https://github.com/sakura-tel/areionskey/commit/1fcfcc82406888a524d27892356ef0cbdf05646f)
- モバイル: 非ログイン時のWelcome画面の ログイン リンクを 新規登録 リンクと同じ場所に移動 [92320b0](https://github.com/sakura-tel/areionskey/commit/92320b047efdbf5979964ca3d469a8ce3bfe659b)
- 依存関係の更新

### ❌Abolitions
- 非ログイン時のユーザ画面 から トレンド関連 を削除 [495c479](https://github.com/sakura-tel/areionskey/commit/495c479ba3f6bb54c26f863f2aadf5d064c62844)

1.6.0 (2022/11/11)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動

Dockerfiles での Node デフォルトバージョンが 18.9.0 から 18.10.0 になっています

### ✨Improvements
- フォロワー解除機能 を追加 by @atsu1125 [PR#912](https://github.com/sakura-tel/areionskey/pull/912)
- サイレンスされたユーザからのフォローは フォローリクエストを発行する機能 を追加 by @atsu1125 [PR#872](https://github.com/sakura-tel/areionskey/pull/872)

### 🐛Fixes
- 投票しようとした時 確認するように変更 by @atsu1125 [PR#934](https://github.com/sakura-tel/areionskey/pull/934)
- 管理者が 自分以外の投稿を削除しようとした時 確認するように変更 by @atsu1125 [PR#913](https://github.com/sakura-tel/areionskey/pull/913)
- ドライブ上限を超過した時 エラーを Bad Request に修正 by @atsu1125 [PR#809](https://github.com/sakura-tel/areionskey/pull/809)
- ブロック時に フォロワーを解除するように変更 by @atsu1125 [f2d6f2a](https://github.com/sakura-tel/areionskey/commit/f2d6f2ad16b3bae1e43d285eebac741a156910fa)
- ナビゲーションに フォローリクエストを常に表示するように変更 [2135d8e](https://github.com/sakura-tel/areionskey/commit/2135d8ed44009b9e87b1ec16d7eb94b7f7895460)
- 言語ファイル・文書の更新
- 依存関係の更新

### ❌Abolitions
- 非ログイン時のWelcome画面 から トレンド関連 を削除 [17f8e24](https://github.com/sakura-tel/areionskey/commit/17f8e2492dd3699b33d148e531a057cf05efd922)
- Revert [3de1369](https://github.com/sakura-tel/areionskey/commit/3de1369778cdc5f2444dedb5200ae80643693965)

1.5.0 (2022/09/15)
--------------------
### To Update
以下を実施してください
- Areionskey 再起動
- database マイグレーション

Dockerfiles での Node デフォルトバージョンが 17.3.0 から 18.9.0 になっています

### ✨Improvements
- パスワードリマインダ を追加 by @atsu1125 [PR#799](https://github.com/sakura-tel/areionskey/pull/799)
- 通報受信メール送信機能 を追加 by @atsu1125 [PR#796](https://github.com/sakura-tel/areionskey/pull/796)
- api/server-info, api/ping を追加 by @atsu1125 [PR#795](https://github.com/sakura-tel/areionskey/pull/795)
- ErasticSearch なしの検索機能 を追加 by @atsu1125 [PR#794](https://github.com/sakura-tel/areionskey/pull/794)

### 🐛Fixes
- nodeinfo の software を areionskey に変更 by @atsu1125 [PR#728](https://github.com/sakura-tel/areionskey/pull/728)
- 左右のナビゲーションバー を整理 [5474635](https://github.com/sakura-tel/areionskey/commit/5474635320b6a38af8c2a99b34b231c73704628d)
- みつける で 無限に もっと見る が出現されないように変更 [3fc4528](https://github.com/sakura-tel/areionskey/commit/3fc45280810a9dbdfde3970a8159937fda403030)
- 依存関係の更新

### ❌Abolitions
- ナビゲーションバーやメニュー から ハイライト を削除 [ad1fb5f](https://github.com/sakura-tel/areionskey/commit/ad1fb5f78aff442a9d8c3aa4d844c8eb5e09ff42)

1.4.0 (2022/06/19)
--------------------
### ✨Improvements
- Misskey の表記 を Areionskey に変更（破壊的変更をされない箇所のみ）
- `:` だけを入力したときに絵文字をサジェストしないように変更

### 🐛Fixes
- ルーム機能の3D描画が出来なくなっていたのを修正
- 猫耳の色を文字色と同色 に変更
- 依存関係の更新
- 言語ファイル・文書の更新

### ❌Abolitions
- ヘッダ から ハイライト を削除
- みつける から 人気のユーザー と 人気のタグ を削除

1.3.8 (2022/06/12)
--------------------
### ✨Improvements
- めいv11 Commit [224cfe95ce5e3c0bfd94c13e1ea5384bb8c3dc8c](https://github.com/mei23/misskey-v11/commit/224cfe95ce5e3c0bfd94c13e1ea5384bb8c3dc8c) までをマージ
- Docker Container 構築時の Alpine Linux を v3.15 に変更

### 🐛Fixes
- モバイルUIの投稿フォームにある絵文字ピッカーアイコンに文字が被る問題を修正
- 猫耳の色を修正（というか復元）

### ❌Abolitions
- メンションのアバター表示（セキュリティアップデートを優先ゆえに実装を後で考える）

1.3.7 (2022/02/13)
--------------------
### ✨Improvements
- モバイルUIの投稿フォームに絵文字ピッカーを追加 ([#167](https://github.com/sakura-tel/areionskey/issues/167))
- プレミアム会員のドライブ増量機能を追加 ([#143](https://github.com/sakura-tel/areionskey/issues/143))
- 投稿フォームの表示を統一・改良 ([#5](https://github.com/sakura-tel/areionskey/issues/5)) ([#232](https://github.com/sakura-tel/areionskey/issues/232))

### 🐛Fixes
- メンションのアバター表示を中揃えに修正 ([#168](https://github.com/sakura-tel/areionskey/issues/168))
- 猫耳の色を修正 ([#130](https://github.com/sakura-tel/areionskey/issues/130))
- ノート中の KaTeX 表記が表示されない点を修正 ([#231](https://github.com/sakura-tel/areionskey/issues/231))
- デスクトップUIのヘッダにあるアナログ時計が見にくい点を修正 ([#233](https://github.com/sakura-tel/areionskey/issues/233))

1.3.6 (2022/02/12)
--------------------
### ✨Improvements
- タグ めいv11 [11.37.1-20220211194000](https://github.com/mei23/misskey-v11/releases/tag/11.37.1-20220211194000) をマージ
- 依存関係の更新
- 言語ファイル・文書の更新

1.3.5 (2022/01/14)
--------------------
### ✨Improvements
- メンションにアバターを表示 ([#17](https://github.com/sakura-tel/areionskey/issues/17))
- プレミアムアカウント・公式アカウントの表示を改良 ([#110](https://github.com/sakura-tel/areionskey/issues/110))
