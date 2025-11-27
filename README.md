# 偏愛会議
偏った愛（趣味）を持つ人同士でも繋がれる場を提供したいとの思いから作成したチャットアプリである。

## 概要
- 開発体系：チーム開発（ハッカソン）
- 制作期間：2ヶ月
- メンバー：5名
- 担当ポジション：バックエンド

## 前提条件
- 目標：Webアプリ開発の経験がない人

## 背景
「趣味を話したいけれど、同じ趣味を持っている人がいない」、「熱量がすごくて、周囲の人から引かれるかもしれない」等の不安を抱えている人に対して、気軽にチャンネルを立ち上げ、共通の趣味を持つ人と繋がれる場を提供したいと思い、本チャットアプリを作成した。

## ターゲット
- 周囲に自分と同じ趣味を持つ人がいない人
- 知人に共有しづらい趣味を持つ人
- 自分の好きな趣味に対して、熱量の高い人との交流を求めている人

## 使用技術
### インフラ
- Docker

### フロントエンド
- HTML・CSS

### バックエンド
- MySQL
- Python

### フレームワーク・ライブラリ
- Flask
- Jinja2

**最初に環境変数ファイル（.env）を作成します**
- Mac、Windows(PowerShell、Git Bash)の場合
```
cp .env.example .env
```
- Windows(コマンドプロンプト)の場合
```
copy .env.example .env
```

**起動方法**
```
docker compose up
```

**ブラウザで確認**
```
http://localhost:55000
```


### ディレクトリ構成
```
.
├── ChatApp              # サンプルアプリ用ディレクトリ
│   ├── __init__.py
│   ├── app.py
│   ├── models.py
│   ├── static          # 静的ファイル用ディレクトリ
│   ├── templates       # Template(HTML)用ディレクトリ
│   └── util
├── Docker
│   ├── Flask
│   │   └── Dockerfile # Flask(Python)用Dockerファイル
│   └── MySQL
│       ├── Dockerfile  # MySQL用Dockerファイル
│       ├── init.sql    # MySQL初期設定ファイル
│       └── my.cnf
├── .env.example         # 環境変数ファイル（.env）を作成する為のサンプルファイル
├── docker-compose.yml   # Docker-composeファイル
└── requirements.txt     # 使用モジュール記述ファイル

```# hackathon-Gteam
