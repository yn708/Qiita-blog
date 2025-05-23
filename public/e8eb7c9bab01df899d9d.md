---
title: 【個人開発】ファッションをサポートするWebアプリを開発しました
tags:
  - Django
  - Webアプリケーション
  - 個人開発
  - Next.js
private: false
updated_at: '2025-02-15T22:40:13+09:00'
id: e8eb7c9bab01df899d9d
organization_url_name: null
slide: false
ignorePublish: false
---
## はじめに
はじめまして。yn[(@yamahon708)](https://x.com/yamahon708)と申します。

この度、『[VIRTUAL CLOSET](https://www.virtual-closet.jp/about)』というWebアプリケーションをリリースいたしました。
以下、サービス概要や今後の展望などを紹介しますので、ぜひご覧ください。

### サービスURL
https://www.virtual-closet.jp/about

https://github.com/yn708/Virtual-Closet


## サービス概要

「Virtual Closet」は、仮想空間にMyクローゼットを作成し、服やコーディネートの管理を簡単に行えるサービスです。

簡単なステップでご利用いただけます。
1. アカウント作成（Google、Emailによるアカウント作成が可能）
2. ファッションアイテムの登録
3. コーディネートの登録

今後の展望として、以下のサービスも提供できるようにする予定です。
- シチュエーションに合わせたコーディネートの自動提案
- おすすめアイテムの提案により、簡単におしゃれを楽しめる仕組み
- SNS機能で他のユーザーのコーディネートを参考にできる
- お気に入り登録や保存機能で簡単に見返しが可能
- コーディネートの予定管理や計画機能

おしゃれが難しいと感じている方も、おしゃれが好きな方も、どなたでもご利用いただけるWebアプリです。ぜひご活用ください。


## 開発背景
私自身、趣味の一環としてファッションが好きで、買い物やコーディネートを考えることが多いのですが、以下のような悩みに直面することがありました。

- コーディネートを組むのに時間がかかる
- 毎回同じコーディネートになってしまう
- シーンに応じたコーディネートが難しい
- 所有しているアイテムや、過去に組んだお気に入りのコーディネートが思い出せない
- 古いアイテムが埋もれており、それを使ったコーディネートを考えるのが面倒
- 時々、おしゃれの感覚がわからなくなる

これらの悩みは、多くの人が日々抱えている問題だと思います。
そこで、このような悩みを持つ方々に向け、以下のようなサービスがあれば良いのではないかと考えました。
- アイテムやコーディネートの管理を簡単にする
- コーディネートやアイテムの提案を行う
- 誰でも簡単におしゃれなコーディネートができる
- 他の方のコーディネートを簡単に参考にできる

類似サービスとして『WEAR』などが思い浮かぶかもしれませんが、本サービスでは、所有アイテムを組み合わせたコーディネートの自動提案機能や、管理方法の工夫、その他の機能によって差別化を図ろうとしています。



### このサービスへの思い

先述の悩みを解決するサービスであると同時に、おしゃれに自信がなく、ファッションに挑戦できない方々にも利用していただけるサービスとなればと考えています。
そのため、今後は『おすすめアイテムの提案』『コーディネート自動提案機能』『SNS機能』といった重要な機能の追加を検討しています。提案機能の精度向上はもちろん、コミュニティ機能の充実も図っていきたいと考えています。


## ユーザー層について
対象ユーザー：すべての方

特に以下のような方におすすめです。
- おしゃれが好きな方
- 服の管理が大変だと感じている方
- おしゃれが難しいと感じている方
- 毎日のコーディネート選びが億劫な方


## 機能一覧

### ▼ ファッションアイテムの登録
<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/eb997b18-bfad-4fa5-9f9d-51ee7771bb4d.gif" width="250">

**1. ファッションアイテムの画像を撮る**（アイテムが目立つように撮影してください）
 
**2. 撮影した画像をフォームに追加し、切り抜きおよび背景除去を実施する**
背景除去を行うことで、コーディネート作成時の見栄えが向上します。
※ 撮影画像が複雑な場合、背景除去がうまく行えないことがあります。背景がシンプルで、被写体がはっきり写っている画像を使用すると、よりきれいに処理できます。なお、iPhone標準搭載の被写体切り抜き機能も便利です。

**3. その他の詳細情報（カテゴリー、ブランド、価格帯、色、柄、シーズン、所有の有無、古着の有無）を登録**
（画像とカテゴリーのみ必須）

**4. 保存ボタンを押して作成完了**



### ▼ コーディネートの登録
登録方法がは２パターンあります。
1. コーディネートの画像をアップロード
2. 登録済みファッションアイテムを組み合わせて作成

|画像アップロード|アイテム組み合わせ|
|:---:|:---:|
|<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/37dd758e-8437-442d-a9e5-bfbef55d08c9.jpeg" width="250">|<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/81a32b4d-1301-4c5b-b285-5d8f4bb46211.gif" width="250">|

その他、シーン、テイスト、シーズンなどの詳細情報は任意で登録可能です。


### ▼ ユーザー機能

ユーザー登録を行うと、各種機能をご利用いただけます。
EmailまたはGoogleアカウントで簡単に登録できます。

<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/830a62fb-26b1-42b4-9eb0-c463ca6bfcb0.jpeg" width="250">


### ▼ お問合せ機能

ユーザー登録をしていなくてもお問い合わせは可能です。（Emailおよび名前を入力していただければOKです）
機能の要望など、さまざまなお問い合わせに対応いたします。
運営側にはEmailやLINEで通知が届くため、迅速に対応いたします。

<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/2b8052cb-67ae-4533-8af0-2477303d1ee5.jpeg" width="250">


### ▼ プロフィール編集機能

プロフィール画像、ユーザー名、名前、生年月日、性別、身長を登録できます。
今後、パーソナライズされた機能提供のために利用する予定です。

<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/01361059-a49c-4937-ab0c-38c41450a645.jpeg" width="250">


### ▼ ダークモード

夜間でも目に優しいカラーでご利用いただけます。

<img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/d2a12e86-8703-4615-8975-6f2eaaaf19b3.jpeg" width="250">


### 追加予定の機能
#### アイテム・コーディネート提案機能
- AIを活用し、登録されたアイテムから最適なコーディネートを提案
- シーン、気温、好みのテイストに応じた提案が可能に
- トレンドアイテムやユーザーの好みに合わせた新規アイテムの提案


#### SNS機能
- 他のユーザーのコーディネートを閲覧、いいね、保存可能
- フォロー機能でお気に入りのユーザーのコーディネートをチェック
- 好みのコーディネートを検索可能


#### コーディネート管理の強化
- 着用予定のコーディネートを日付別に管理（カレンダー機能）
- スタイルブックなどのコーディネート集の作成
- 旅行時などのコーディネート管理


#### その他
お気に入り登録や保存機能など、UX向上のための各種機能


## 工夫した点
### UI/UX視点
ユーザーの動線を意識して開発を進めました。

- **待機時間の工夫**
例えば、ファッションアイテム登録時に画像選択後、画像の最適化や背景除去などのバックエンド処理が行われる際、ユーザーに待機時間が生じる問題がありました。そこで、画像処理中はLoading表示を行い、その他の詳細情報の入力を並行して行えるよう工夫しました。
　
- **ダークモード実装**
昼夜問わず使用されることを想定し、夜間でも目に優しいダークモードを実装しました。特に、夜間にスマートフォンを操作される方には、ダークモードをご活用いただければ幸いです。
　
- **レスポンシブデザインによるマルチデバイス対応**
当然ながらレスポンシブ対応も実施しました。デスクトップでの利用が見やすいとはいえ、基本的にはスマートフォンでの操作が中心であることから、各デバイスに合わせた実装を行っています。


### 認証機能
フロントエンドではNextAuth.jsを、バックエンドではdj-rest-authおよびdjango-allauthを使用し、Google認証に加えてEmail認証も実現しました。Email認証では、認証コードの送信（再送信）による二段階認証（ワンタイムパスワード方式）を採用し、パスワード再設定機能も実装しています。

- **リフレッシュトークンの設定**
単なるトークンの使用にとどまらず、リフレッシュトークンを利用することで安全性を向上させました。

### 画像処理
画像を主に扱うサービスであるため、以下の処理を実施しています。

- 画像の圧縮
- 画像の変換（HEICなど　→ WebP）
- 切り抜き処理
- 背景除去処理
- Canvasによる画像生成

今回、画像の保存先としてS3を、さらにCloudFrontも利用しています。サービス継続のため、無駄なコストがかからないよう努めました。
特に、画像容量については、最大サイズを小さく設定しているため、画質に妥協がある点は今後の設定見直しを検討する可能性があります。
背景除去に関しては、当初はrembgを用いて実装していましたが、ライブラリが大きいという問題があったため、OpenCVを採用し負荷軽減を図りました。さらに、クライアント側のデバイスによる処理可否を考慮し、できるだけサーバーサイドで処理を行うようにしています。

また、iPhoneで使用する場合、画像形式がHEICであることが多いため、対応可能な形式に変換しています。さらに、単にJPEGやPNGを使用するのではなく、圧縮効率が高く画質をほとんど損なわずにファイルサイズを軽量化できるWebPを採用しました。

## 主な使用技術

| カテゴリー        | 使用技術          |
| :---------------| :----------------|
| フロントエンド        　|Next.js <br>React <br>  TypeScript  |
| バックエンド            |Django <br> Python                |
| DB                    | PostgreSQL                       |
| インフラ                | Vercel / Render / neon          |
| 画像ストレージ           | S3 / CloudFront               |
| 認証             |NextAuth.js <br/> dj-rest-auth / django-allauth|
| 開発環境               | Docker                       |
| CI/CD                 | GitHub Actions               |
| テスト             | Jest / React Testing Library <br/>  pytest|
| コード解析 / フォーマッター | ESLint / Prettier <br/>  Ruff|
| UI / CSS           |shadcn/ui   　/　 Tailwind CSS |
| その他（フロントエンド） |Zod / heic2any / date-fns-tz / react-easy-crop / browser-image-compression など|
| その他（バックエンド）   |  Pillow / OpenCV　など|

## インフラ構成

![VC_インフラ構成図.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/5c9ad3dc-d98b-4758-b7ea-ab7b2142626a.png)


## 技術選定理由

### フロントエンド: Next.js / React / TypeScript
**検討技術**： Vue.js / Nuxt.js
**採用理由**：

- Next.js / React：
デファクトスタンダードであり、SSR/SSGによるパフォーマンス向上とSEO最適化が可能。さらに、Vercelとの親和性が高く、デプロイが容易であり、React Server Componentsもサポートしているため採用。
　
- TypeScript：
型安全性による開発時のエラー検出、コードのメンテナンス性向上、そしてTypeScriptの使用が当たり前になりつつあるため採用しました。


#### UI/CSSフレームワーク関連：shadcn/ui , Tailwind CSS
**採用理由**：
人気が高くカスタマイズ性に優れており、Tailwind CSSを用いることで簡単にデザインの調整が可能です。また、TypeScriptのサポートも充実しているため選定しました。


### バックエンド: Django / Python
**検討技術**： Ruby / Ruby on Rails, FastAPI
**採用理由**：

- Python（言語選定理由）:
今後、AIによるアイテム・コーディネートの自動提案や画像処理の需要が見込まれるため、AI分野やデータ分析、画像処理に強いPythonを採用しました。


- Django（フレームワーク選定理由）：
過去の使用経験によりランニングコストの低減、dj-rest-authおよびdjango-allauthによる認証機能の実装の容易さ、さらにDjango REST Frameworkによる効率的なAPI開発が理由です。


### インフラ: Vercel / Render / neon
**検討技術**： AWS(ECR, ECS, RDS等)
**採用理由**：

- Vercel： Next.jsとの親和性が高く、デプロイが容易であるため。
- Render：コンテナ化されたバックエンドのデプロイが容易で、コスト面でも安価または無料のプランが利用できるため。
- neon：サーバーレスPostgreSQLであり、スケーリングが容易（無料枠から開始可能）な点が魅力です。


なお、AWSは柔軟ではあるものの設定が複雑で料金も高いため、現時点では採用していません。将来的にユーザー数が増加し、さらなる柔軟性が求められる場合は、AWSへの切り替えを検討する可能性があります。


### 画像ストレージ: S3, CloudFront
**検討技術**： Google Cloud Storage
**採用理由**：

今後、インフラ環境をAWSに統一する際にも管理が容易になり、CloudFrontとの連携により最適化が可能で、料金も比較的安価なため採用しました。


### CI / CDツール : GitHub Actions
**検討技術**： CircleCI
**採用理由**
普段利用しているGitHubとの親和性が高く、開発体験の向上が期待できる点、また、CircleCIでのセキュリティインシデントやGitHub Actionsの支持率の増加も理由として挙げられます。


### 認証 : NextAuth.js, dj-rest-auth / django-allauth
**採用理由**
実装が容易で、Google認証に加えEmail認証やパスワードリセットなどの機能が備わっているため。NextAuth.jsは既に使用経験があり、学習コストが低いことも選定理由です。


### 開発環境 : Docker、GitHub
**採用理由**
実務で広く利用されている技術であり、個人開発においても大きな役割を果たすため採用しました。



## ER図

![VC_ER図.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/3470689/ccdba867-2356-4071-ab71-0aac8b55c8b8.png)



## おわりに
Virtual Closetは、私自身のファッションへの思いと、多くの方々が抱えるコーディネートの悩みを解決したいという想いから生まれました。このサービスを通じて、ファッションを楽しむ人が増えることを願っています。
現在はベーシックな機能のみの提供となっていますが、今後はAIを活用した提案機能やSNS機能など、より便利で魅力的な機能を追加していく予定です。ユーザーの皆様からのフィードバックを大切にしながら、サービスの改善と発展に努めてまいります。
最後に、本サービスをご利用いただいている皆様に心より感謝申し上げます。より良いサービスとなるよう、機能改善やアップデートを継続的に行っていきますので、今後も本サービスを使用していただければ幸いです。
ご要望やご意見がございましたら、お問い合わせフォームよりお気軽にご連絡ください。皆様のご意見を参考に、より使いやすく、より便利なサービスへと成長させていきたいと考えております。
