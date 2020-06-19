# Blockly [![Build Status]( https://travis-ci.org/google/blockly.svg?branch=master)](https://travis-ci.org/google/blockly)


GoogleのBlocklyは、Webベースのビジュアルプログラミングエディターです。ユーザーはブロックを一緒にドラッグしてプログラムを構築できます。すべてのコードは無料でオープンソースです。

**プロジェクトページは https://developers.google.com/blockly/**

![](https://developers.google.com/blockly/images/sample.png)

BBlocklyにはアクティブな [開発者フォーラム](https://groups.google.com/forum/#!forum/blockly)があります。 早くプロトタイプを見せてください。集合的に私たちは多くの経験を持ち、時間を節約するヒントを提供できます。私たちはフォーラムを積極的に監視し、通常2営業日以内に質問に回答します。

[Blocklyで何をしているのか](https://developers.google.com/blockly/registration)教えてください。アンケートは数分で完了し、Blocklyコミュニティをよりよくサポートするのに役立ちます。

クロスブラウザテストプラットフォームとオープンソース<3は [Sauce Labs](https://saucelabs.com)が提供しています。

IE11をサポートし、 [BrowserStack](https://browserstack.com)を使用してテストします。

貢献したいですか？すごい！まず、 [投稿者向けガイドライン](https://developers.google.com/blockly/guides/modify/contributing).をお読みください。

## リリース

次のメジャーリリースは2020年6月26日です。**.

最新のコードをマスターブランチにプッシュしてリリースし、続いて [docs](https://developers.google.com/blockly) と [demo pages](https://blockly-demo.appspot.com)を更新します。
通常、四半期ごと（3か月ごと）に新しいバージョンのBlocklyをリリースします。標準アクションの実行時のクラッシュや、Blocklyが使用できなくなるレンダリングの問題などの重大なバグがある場合は、リリース間でマスターに修正をチェリーピックして修正します。
[リリースページ](https://github.com/google/blockly/releases) すべてのリリースのリストを持っています。

リリースにはリリース日（YYYYMMDD）のタグが付き、先頭に「2」が付きます。メジャーバージョンまたはマイナーバージョン（[2.20190722.1](https://github.com/google/blockly/tree/2.20190722.1)のような）が必要な場合に備えて、末尾の「.0」。npmを使用している場合は、npmにblocklyパッケージをインストールできます。
```bash
npm install blockly
```

### 新しいAPI

新しいAPIがマスターにマージされると、次のリリースまでベータ版と見なされます。通常、マスターにマージされた後はAPIを変更しないようにしますが、APIの使用方法を確認した後で変更を加える必要がある場合があります。APIが少なくとも2つのリリースで使用されている場合は、破損しないように最善を尽くします。

未リリースのAPIは大幅に変更される可能性があります。developに入っているがmasterに入っていないものは、予告なしに変更される可能性があります。

### ブランチ

There are two main branches for Blockly.

**[master](https://github.com/google/blockly)** - This is the (mostly) stable current release of Blockly.

**[develop](https://github.com/google/blockly/tree/develop)** - This is where most of our work happens. Pull requests should always be made against develop. This branch will generally be usable, but may be less stable than the master branch. Once something is in develop we expect it to merge to master in the next release.

**other branches:** - Larger changes may have their own branches until they are good enough for people to try out. These will be developed separately until we think they are almost ready for release. These branches typically get merged into develop immediately after a release to allow extra time for testing.

## Issues and Milestones

We typically triage all bugs within 2 working days, which includes adding any appropriate labels and assigning it to a milestone. Please keep in mind, we are a small team so even feature requests that everyone agrees on may not be prioritized.

### Milestones

**Upcoming release** - The upcoming release milestone is for all bugs we plan on fixing before the next release. This typically has the form of `year_quarter_release` (such as `2019_q2_release`). Some bugs will be added to this release when they are triaged, others may be added closer to a release.

**Bug Bash Backlog** - These are bugs that we're still prioritizing. They haven't been added to a specific release yet, but we'll consider them for each release depending on relative priority and available time.

**Icebox** - These are bugs that we do not intend to spend time on. They are either too much work or minor enough that we don't expect them to ever take priority. We are still happy to accept pull requests for these bugs.
