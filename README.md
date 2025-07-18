# 🍼 育児質問アプリ

子どもの栄養と睡眠に関する質問に答えるAIアプリです。AI専門家があなたの子育ての疑問にお答えします。

## 🌟 機能

### 🥗 子どもの栄養モード
- 子どもの健康な発育を支える食事や栄養バランスについてアドバイス
- 年齢に応じた栄養素の必要量や食事のポイントを提供
- 科学的根拠に基づいた実践的な内容

### 😴 子どもの睡眠モード
- 子どもの睡眠習慣や睡眠の問題についてアドバイス
- 年齢に応じた適切な睡眠時間、睡眠環境の整え方
- 睡眠リズムの改善方法などを含む具体的なアドバイス

## 🚀 デプロイ方法

### Streamlit Cloudでのデプロイ

1. [Streamlit Cloud](https://streamlit.io/cloud)にアクセス
2. GitHubアカウントでサインイン
3. 「New app」をクリック
4. リポジトリ: `gorimatsuchiyo/STREAMLIT-LLM-APP`
5. ブランチ: `main`
6. メインファイル: `app.py`
7. 「Advanced settings」で環境変数を設定：
   - `OPENAI_API_KEY`: あなたのOpenAI APIキー
8. 「Deploy!」をクリック

### ローカル実行

```bash
# 必要なパッケージをインストール
pip install -r requirements.txt

# .envファイルを作成してAPIキーを設定
echo "OPENAI_API_KEY=your_api_key_here" > .env

# アプリを起動
streamlit run app.py
```

## 🛡️ セキュリティ

- OpenAI APIキーは環境変数で管理
- `.env`ファイルは`.gitignore`で除外
- 本番環境では環境変数またはStreamlit Cloudの設定で管理

## 📋 必要な環境変数

- `OPENAI_API_KEY`: OpenAI APIキー

## 🔧 技術スタック

- **フロントエンド**: Streamlit
- **AI/ML**: LangChain + OpenAI GPT-3.5-turbo
- **環境管理**: python-dotenv
- **デプロイ**: Streamlit Cloud
