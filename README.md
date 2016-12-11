# 使い方
次のようにコミットメッセージの先頭につけます。`:emoji: commit message`

例えば、README.txtを追加した場合は`:memo: Add README.txt`などと書くようにします。

# 絵文字(Emoji)
絵文字とコミットタイプの対応は以下の通りです。

Emoji| コミットタイプ
--|--
✨ `:sparkles:` |新規機能追加
📝 `:memo:` |ドキュメント追加
🔉 `:sound:`|ログ追加
✅ `:white_check_mark:`|テストの追加
👍 `:+1:`|機能修正
🚀  `:rocket:` |パフォーマンス改善
👮  `:cop:`|セキュリティ関連の改善
✏️ `:pencil2:`|タイポなどの修正
🎨 `:art:`|リファクタリング
🚧 `:construction:`|コメントアウトなど
🔥 `:fire: `|ファイル削除
🔇  `:mute:`|ログ削除
🐛 `:bug:` |バグ修正
🔖  `:bookmark:` |バージョンアップ
🎉 `:tada:`|イニシャルコミット

# コミットメッセージの種別
コミットのメッセージとその意味の対応は以下の通りです。

コミットメッセージ | 意味
--|--
Add| 新規(ファイル)機能追加
Update| 機能修正、既存機能追加（バグではない）
Clean|リファクタリング
Remove|削除など
Fix|バグ修正
Upgrade|バージョンアップ

# 絵文字を自動補完してgit commit
Atomを使用している場合は、[git-plus](https://atom.io/packages/git-plus)と[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)を併用すると絵文字の入力が楽になります。


# ターミナル上でgit commit
ターミナル上で絵文字を手打ちする場合にはテンプレートとして絵文字リストを登録しておくと便利です。
テンプレートの登録は以下のように行います。
```
cd emoji-matome
cp .gitmessage.txt ~/.gitmessage.txt
git config --global commit.template ~/.gitmessage.txt
```

これで`git commit`コマンド後に`.gitmessage.txt`がテンプレートとしてターミナル上に表示されるようになります。
