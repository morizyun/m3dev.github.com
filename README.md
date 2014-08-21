### Tech side of M3 #m3dev

こちらでアクセスできます。English version coming soon.

http://m3dev.github.io/

### このサイトの運用について

typo の修正やコンテンツの追加は以下のようにして行ってください。

#### 修正方法

fork してから develop ブランチに対して pull request してください。

Middleman を使っています。

http://middlemanapp.com/

```
gem install bundler
bundle install
bundle exec middleman server
```

で http://localhost:4567/ にブラウザからアクセスできます。

#### M3 Tech Talk

発表のデータは `data/talks.yml` に追記してください。これをもとにページを生成します。

- `title`: タイトル
- `by`: 発表者名
- `github_id`: （発表者の GitHub ID）
- `type`: スライドの種類（speakerdeck, slideshare, html, link に対応しています）
- `source`: スライド表示用のデータ（`type` が speakerdeck, slideshare, html の場合は、HTML。link の場合は URL。）

YAML の文字列中に `:` を書く際は文字列全体を `''` で囲ってください。`title` や Slideshare 用の `source` で `:` が入りがちです。

#### デプロイ方法

GitHub の develop ブランチに push すると、Wercker が自動でデプロイしてくれます。
