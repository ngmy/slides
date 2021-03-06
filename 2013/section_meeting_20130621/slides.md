# 継続的インテグレーションのすゝめ

2013年6月21日

永宮　悠大



## 継続的インテグレーション

> チームのメンバーが各自の成果物を頻繁に統合するソフトウェア開発のプラクティスである。
> 通常、最低でも1日に1度以上は各自でインテグレーション作業を行う。
> インテグレーション時のエラーをできるだけ早く検出できるよう、すべてのインテグレーションは、
> テストを含めた自動化されたビルドによって検出される。

![ci_beginner](images/ci_beginner.jpg)


## イメージ

![ci_overview](images/ci_overview.png)



## 期待できる効果


## 開発を効率化します


## というのは嘘で・・・


## 仕様変更が頻繁に発生する開発を効率化します


## 開発コストのイメージ

![ci_effect](images/ci_effect.png)


## 迅速なフィードバックを可能にします


## ビルド状況

![phpundercontrol_projects](images/phpundercontrol_projects.png)

* ビルド成功時はグリーン、失敗時はレッドになる
* リポジトリ単位でプロジェクトを作成可能


## 単体試験

![phpundercontrol_phpunit](images/phpundercontrol_phpunit.png)

* テスト成功時はグリーン、失敗時はレッドになる


## カバレッジ

![phpundercontrol_coverage](images/phpundercontrol_coverage.png)

* カバレッジの度合いを色分けして表示
  * 「高」はグリーン
  * 「中」はイエロー
  * 「低」はレッド
* ファイルごとの実行された行／実行されなかった行も色分けして表示可能


## コーディング規約チェック

![phpundercontrol_phpcs](images/phpundercontrol_phpcs.png)

* プロジェクトで決めたコーディング規約を遵守しているかチェック
* Error（重度な違反）、Warning（軽度な違反）の2段階で指摘


## コード改善

![phpundercontrol_phpmd](images/phpundercontrol_phpmd.png)

* コードの改善点を指摘してくれる
  * メソッドが長すぎる
  * クラスが大きすぎる
  * ロジックが複雑すぎる
  * など


## 品質を視える化します


## ビルドのメトリクス

![phpundercontrol_metrics](images/phpundercontrol_metrics.png)


## 具体例1

![phpundercontrol_metrics_coverage](images/phpundercontrol_metrics_coverage.png)

（´-`）.｡oO（カバレッジが高いので安心だな）


## 具体例2

![phpundercontrol_metrics_coding_violations](images/phpundercontrol_metrics_coding_violations.png)

（´-`）.｡oO（よし、コーディング規約は守られているな）

（´-`）.｡oO（最初の頃はひどかった…）


## 具体例3

![phpundercontrol_metrics_test_to_code_ratio](images/phpundercontrol_metrics_test_to_code_ratio.png)

* 実コードが増えたらテストコードも増えている

  ⇒テストしている

* 実コードが増えたのにテストコードが増えていない

  ⇒テストしていない

（´-`）.｡oO（よし、みんなしっかりテストを書いてるな）


## 具体例4

![phpundercontrol_metrics_build](images/phpundercontrol_metrics_build.png)

* オレンジ（失敗ビルド）が多い

  ⇒開発が盛んに行われている

* グリーン（成功ビルド）が多い

  ⇒軽微な開発が続いている

（´-`）.｡oO（開発もだいぶ落ち着いてきたなぁ）



## 必要なもの

* 継続的インテグレーションツール
  * phpUnderControl
  * CruiseControl
  * Jenkins
  * など
* 継続的インテグレーション用サーバ
* バージョン管理システム
  * Subversion
  * Git
  * など
* テストコード


## 運用フロー例

![ci_workflow](images/ci_workflow.png)



## まとめ


## 継続的インテグレーションの効果

* 仕様変更が頻繁に発生する開発の効率化
* 迅速なフィードバック
* 品質の視える化


## Let's Enjoy Continuous Integration Life!



## Thank You!

BY Yuta Nagamiya
