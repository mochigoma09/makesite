# AI Webサイト生成 ＆ 完全自動公開 (AI画像選定版)

テキストで要望を入力するだけで、AI（Gemini）がWebサイトのコードを生成し、Unsplashから最適な画像を自動取得して、GitHub Pagesに完全自動で公開するブラウザ完結型のツールです。

## 🌐 デモページ (Live Demo)

以下のURLから、実際にブラウザ上でツールをお試しいただけます。  
[https://<あなたのユーザー名>.github.io/<リポジトリ名>/](https://<あなたのユーザー名>.github.io/<リポジトリ名>/)

## 特徴
- **AIによる完全自動コーディング**: Gemini APIを利用して、要望に合わせた1ペラのHTML/CSS/JSを生成します。
- **画像自動選定**: Unsplash APIと連携し、要望に合った高品質な画像を自動で検索・組み込みます（任意機能）。
- **GitHub自動公開**: GitHub APIを利用して、リポジトリの作成からコードのPush、GitHub Pagesの公開設定までを全自動で行います。
- **サーバー不要**: バックエンドサーバーを持たず、HTMLファイル1つをブラウザで開くだけで動作します。

## 必要なもの (APIキー)

このツールを利用するには、以下のAPIキー・トークンが必要です。

1. **Gemini APIキー**
   - コードと画像の検索キーワード生成に使用します。[Google AI Studio](https://aistudio.google.com/app/apikey) から取得できます。
2. **GitHub Personal Access Token (PAT)**
   - リポジトリの作成とコードのPushに使用します。`repo` スコープの権限が必要です。GitHub Settings (Classic) から作成してください。
3. **Unsplash Access Key (任意)**
   - 画像の自動取得に使用します。Unsplash Developers からアプリケーションを作成し、Access Keyを取得してください。

## 使い方

1. リポジトリをクローンするか、`index.html` をダウンロードします。
2. `index.html` をお使いのWebブラウザ（Chrome, Edge, Safariなど）で直接開きます。
3. 画面の「基本設定」フォームに以下を入力します。
   - Gemini APIキー
   - GitHub Personal Access Token
   - 作成したいリポジトリ名 (例: `auto-generated-site-01`)
   - Unsplash Access Key (画像を自動取得したい場合)
4. 「どんなWebサイトを作りますか？」のテキストエリアに、作成したいサイトの要望を入力します。
   - 例: `山奥にある静かな温泉旅館のホームページを作って。高級感のある和風のデザインにしてほしい。`
5. 「✨ 全自動で生成 ＆ GitHub公開」ボタンをクリックします。
6. 生成状況が画面上に表示されます。処理が完了すると、作成されたGitHubリポジトリのURLと、公開されたWebサイト（GitHub Pages）のURLが表示されます。

## 注意事項

- Gemini APIの利用制限（無料枠の超過、リクエスト過多）に達するとエラーになります。
- GitHub Pagesの公開処理には、GitHub側の仕様により完了後アクセスできるようになるまで1〜2分程度かかる場合があります。

## ライセンス

このプロジェクトは MIT ライセンスのもとで公開されています。
