概要
このツールは、仕事探しと応募プロセスを効率化するために設計された自動化ツールです。人工知能を活用することで、応募の自動化、求人の提案、カスタマイズされた履歴書の生成が可能です。

主な特徴
応募プロセスの自動化により時間を節約
個人の経歴に基づいた求人の提案
応募に最適化された履歴書やカバーレターを自動生成
マルチプラットフォーム対応（Windows、Ubuntuなど）
インストール方法
1. Pythonのインストール
公式サイトから最新バージョンのPythonをインストールしてください。
詳細な手順は以下のリンクを参照してください。
Python公式サイト

2. Google Chromeのインストール
公式サイトからGoogle Chromeをインストールしてください。
Google Chrome公式サイト

3. リポジトリのクローン
以下のコマンドを実行し、リポジトリをローカル環境にクローンします。

bash
コピーする
編集する
git clone https://github.com/feder-cr/Jobs_Applier_AI_Agent.git
cd Jobs_Applier_AI_Agent
4. 仮想環境の作成と有効化
Unix系:
bash
コピーする
編集する
python3 -m venv virtual
source virtual/bin/activate
Windows:
bash
コピーする
編集する
.\virtual\Scripts\activate
5. 必要なライブラリのインストール
以下のコマンドで必要な依存ライブラリをインストールします。

bash
コピーする
編集する
pip install -r requirements.txt
設定
1. secrets.yaml
APIキーやその他の機密情報を含む設定ファイルです。このファイルを編集し、必要な情報を入力してください。

例:

yaml
コピーする
編集する
llm_api_key: "ここにOpenAIまたはGeminiのAPIキーを入力"
2. plain_text_resume.yaml
履歴書情報を構造化した形式で入力します。

例:

yaml
コピーする
編集する
personal_information:
  name: "山田"
  surname: "太郎"
  email: "yamada@example.com"
  github: "https://github.com/yamada"
  linkedin: "https://www.linkedin.com/in/yamada/"
使い方
設定が完了したら、以下のコマンドでプログラムを実行します。

bash
コピーする
編集する
python main.py
トラブルシューティング
OpenAI API制限エラー
エラー例:

bash
コピーする
編集する
Rate limit reached: You exceeded your current quota.
解決方法:

OpenAIの課金設定を確認し、必要に応じてクレジットを追加してください。
YAML設定エラー
エラー例:

vbnet
コピーする
編集する
yaml.scanner.ScannerError: while scanning a simple key
解決方法:

YAMLファイルのインデントや構文を確認してください。
YAMLバリデータを使用してエラーを特定します。
貢献方法
このプロジェクトはオープンソースです。以下の方法で貢献できます。

プロジェクト管理や改善提案への参加（技術的スキル不要）
コードレビューや新機能の追加（技術的スキルがある場合）
詳細はGitHubの貢献ガイドラインを参照してください。

ライセンス
このプロジェクトはオープンソースで提供されており、自由に利用および変更が可能です。詳細はLICENSEファイルをご覧ください。

