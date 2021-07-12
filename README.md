# 使い方
次のようにコミットメッセージの先頭につけます。`:emoji: 動詞: メッセージ`  

例えば、README.txtを追加した場合は`:memo: Add: Create README.txt`などと書くようにします。  

# 絵文字(Emoji)
絵文字とコミットタイプの対応は以下の通りです。  

| Emoji                   | コミットタイプ         | 対応する動詞 |
| :---------------------- | :--------------------: | :----------: |
| ✨ `:sparkles:`         | 新規機能追加           | Update, Add  |
| 📝 `:memo:`             | ドキュメント追加       | Update, Add  |
| 🔉 `:sound:`            | ログ追加               | Update, Add  |
| ✅ `:white_check_mark:` | テストの追加           | Update, Add  |
| 👍 `:+1:`               | 機能修正               | Fix, Update  |
| 🚀 `:rocket:`           | パフォーマンス改善     | Fix, Update  |
| 👮 `:cop:`              | セキュリティ関連の改善 | Fix, Update  |
| ✏️ `:pencil2:`          | タイポなどの修正       | Clean        |
| 🎨 `:art:`              | リファクタリング       | Clean        |
| 🚧 `:construction:`     | コメントアウトなど     | Remove       |
| 🔥 `:fire:`             | ファイル削除           | Remove       |
| 🔇 `:mute:`             | ログ削除               | Remove, Fix  |
| 🐛 `:bug:`              | バグ修正               | Fix          |
| 🔖 `:bookmark:`         | バージョンアップ       | Upgrade      |
| 🎉 `:tada:`             | イニシャルコミット     |              |

# 絵文字を自動補完してgit commit
Atomを使用している場合は、[git-plus](https://atom.io/packages/git-plus)と[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)を併用すると絵文字の入力が楽になります。  

# ターミナル上でgit commit
ターミナル上で絵文字を手打ちする場合にはテンプレートとして絵文字リストを登録しておくと便利です。  
テンプレートの登録は以下のように行います。  

絵文字付き:  
```shell
wget -O ~/.gitmessage.txt https://raw.githubusercontent.com/TwoSquirrels/commit-template/master/.gitmessage_with_emoji.txt ; git config --global commit.template ~/.gitmessage.txt
```

絵文字抜き:  
```shell
wget -O ~/.gitmessage.txt https://raw.githubusercontent.com/TwoSquirrels/commit-template/master/.gitmessage.txt ; git config --global commit.template ~/.gitmessage.txt
```

これで`git commit`コマンド後に`.gitmessage.txt`がテンプレートとしてターミナル上に表示されるようになります。  
