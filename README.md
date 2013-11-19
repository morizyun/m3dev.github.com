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

#### デプロイ方法

m3dev のメンバーのみが可能な作業です。

develop ブランチで修正が終わったら `middleman deploy` を実行すると master ブランチに build した静的ファイルを反映します。


