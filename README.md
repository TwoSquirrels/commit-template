# コミットメッセージの先頭に使う絵文字(Emoji)まとめ

例えば、バグを修正したというコミットメッセージだけでも、チームや人によって"fix bug", "bug fixed", "fixed bug", "bug fix"など、さまざまな可能性がある。そこで、それぞれのコミットに対応した絵文字(Emoji)を使うことで、一目見ただけでコミットの種類をわかりやすく伝えることができる。 😄

自分用の簡易絵文字チートシートとして残しておく。

### 使い方
次のようにコミットメッセージの先頭につける。`:emoji: commit message`

### 絵文字(Emoji)

コミットタイプ | Emoji
----------      | -------------
コードのフォーマットや構造の改良|🎨 `:art:`
パフォーマンス | 🐎 `:racehorse:`
メモリリークの改善| 🚱 `:non-potable_water:`
ドキュメント | 📝 `:memo:`
Linux用の何かしらを改善| 🐧 `:penguin:`
Mac OS用の何かしらを改善| 🍎 `:apple:`
Windows用の何かしらを改善| 🏁 `:checkered_flag:`
バグ修正 | 🐛 `:bug:`
コードやファイルの削除| 🔥 `:fire:`
CIビルドの修正| 💚 `:green_heart:`
テストの追加| ✅ `:white_check_mark:`
セキュリティ| 🔒 `:lock:`
依存関係をアップグレード| ⬆️ `:arrow_up:`
依存関係をダウングレード| ⬇️ `:arrow_down:`
リンターの警告削除| 👕 `:shirt:`
イニシャルコミット | 🎉 `:tada:`
バージョンタグ | 🔖 `:bookmark:`
新機能 | ✨ `:sparkles:`
メタデータ | 📇 `:card_index:`
通常アップデート | ⚡ `:zap:`
その他 | [絵文字チートシート](http://www.emoji-cheat-sheet.com/)

## 絵文字を自動補完してgit commit
基本的に絵文字を手打ちするのは面倒だが、Atomを使用している場合は、[git-plus](https://atom.io/packages/git-plus)と[autocomplete-emojis](https://atom.io/packages/autocomplete-emojis)を併用すると楽。

![](https://zippy.gfycat.com/VigilantHarmfulKestrel.gif)

## ターミナル上でgit commit
ターミナル上で絵文字を手打ちする場合にはテンプレートとして絵文字リストを登録しておくと便利です。
テンプレートの登録は以下のように行います。
```
cp emoji-matome/.gitmessage.txt ~/.gitmessage.txt
git config --global commit.template ~/.gitmessage.txt
```

これで`git commit`コマンド後に`.gitmessage.txt`がテンプレートとしてターミナル上に表示されるようになります。
