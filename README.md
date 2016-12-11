# 使い方
次のようにコミットメッセージの先頭につける。`:emoji: commit message`

# 絵文字(Emoji)

コミット種別 | Emoji| コミットタイプ
--|--|--
Add| ✨ `:sparkles:` |新規機能追加
|📝 `:memo:` |ドキュメント追加
|🔉 `:sound:`|ログ追加
|✅ `:white_check_mark:`|テストの追加
Update|👍 `:+1:`|機能修正
|🚀  `:rocket:` |パフォーマンス改善
|👮  `:cop:` Update|セキュリティ関連の改善
 Clean|🎨 `:art:`|リファクタリング
Disable|🚧 `:construction:`|コメントアウトなどの無効化  
Remove|🔥 `:fire: `|ファイル削除
|🔇  `:mute:`|ログ削除
Fix|🐛 `:bug:` |バグ修正
Upgrade|🔖  `:bookmark:` |バージョンアップ
Initial commit|🎉 `:tada:`|イニシャルコミット

# 絵文字を自動補完してgit commit
基本的に絵文字を手打ちするのは面倒だが、Atomを使用している場合は、[git-plus](https://atom.io/packages/git-plus)と[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)を併用すると楽。

![](https://zippy.gfycat.com/VigilantHarmfulKestrel.gif)

# ターミナル上でgit commit
ターミナル上で絵文字を手打ちする場合にはテンプレートとして絵文字リストを登録しておくと便利です。
テンプレートの登録は以下のように行います。
```
cp emoji-matome/.gitmessage.txt ~/.gitmessage.txt
git config --global commit.template ~/.gitmessage.txt
```

これで`git commit`コマンド後に`.gitmessage.txt`がテンプレートとしてターミナル上に表示されるようになります。
