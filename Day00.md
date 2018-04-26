Day00
===

# ASP.NETとは？

- (一言で言うと)Webアプリケーションを開発するための技術

# クライアントとサーバ(概念の説明)

## クライアント
- *要求を行い、結果を受け取る*コンピュータのこと

## サーバ
- *情報やサービスを提供する*コンピュータのこと
  - 例: メールサーバ、データベースサーバ、Webサーバ等

# リクエストとレスポンス

- plantUMLで図を生成


'''

	@startuml
	' 手書き風
	skinparam handwritten true
	
	' 役者
	actor client
	node Server
	
	' 関係
	client -right-> Server: Request
	Server -left-> client: Response
	@enduml

'''


![リクエストとレスポンスのイメージ図](./img/Day00/001.png)

# 動的なページと静的なページ


'''

@startuml
' 手書き風
	skinparam handwritten true
	
	' 役者
	actor client
	node Server{
		database ASP.NET
		}
	
	' 関係
	client -right-> Server: ［山田］という名前を送信
	ASP.NET -left-> client: 送信した値を結びつけた結果を送信
@enduml

'''


![リクエストとレスポンスのイメージ図](./img/Day00/002.png)

