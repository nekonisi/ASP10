イベントドリブンモデルに関して
---

## このページの概要

- ASP.NETの解説の中で出てきた*イベントドリブンモデル*についてまとめる。

## イベントドリブンモデルの概要

- イベントドリブンモデル is
  - ボタンがクリックされた，カーソルが外れた，といったイベントを引き金に，その後の一連の処理をまとめる方式のこと
  - 対義語は，*リクエストリプライ方式*

## リクエストリプライ方式との比較

項目名|イベントドリブンモデル|リクエストリプライモデル
------|----------------------|------------------------
別名|Orchestration|Choreography
イベント発生のタイミング|各イベントが発生したタイミング|オーケストレーションプログラムのタイミング

### `Orchestration`モデル

- 全体の処理を管理する指揮者にあたるプログラムが存在し，そこからのリクエストによってサービスを実行する。

### `Choreography`モデル

- 個々のサービスにあらかじめ動作条件や次にどのサービスを起動させるかといった設定が与えられており，それに従って，各サービスが自動的に動作する方式である。

[TOPへ](./index.html)