# PrivateSaronn - Document Café ☕

個人的な企画案・技術ドキュメント・アイデアメモを管理・共有するためのリポジトリです。

## 📚 概要

documentsフォルダにHTMLぶっこむと、新しいリンクボタンが生成される。

## 🌐 アクセス

**Document Café**: https://ryotamuraite.github.io/PrivateSaronn/

GitHub Pagesで公開されているドキュメント一覧ページから、各資料にアクセスできます。

## 📁 構成

```
PrivateSaronn/
├── index.html                 # ドキュメント一覧ページ
├── documents/                 # 資料フォルダ
│   ├── metadata.json         # 自動生成されるメタデータ
│   └── *.html                # 各種ドキュメント
├── .github/
│   └── workflows/
│       └── update-metadata.yml # メタデータ自動更新Actions
└── README.md                  # このファイル
```

## 🔧 システム機能

- **自動メタデータ抽出**: HTMLファイルから`<title>`タグを自動抽出して日本語タイトルを表示
- **GitHub Actions連携**: ドキュメント追加時に自動でメタデータを更新
- **動物アイコン**: ファイルごとにユニークな動物アイコンを自動割り当て
- **レスポンシブデザイン**: モバイル・デスクトップ両対応のカフェ風UI

## 📝 更新履歴

### 2025/09/07
- 本ドキュメントを新規作成。
- タイトルの自動検出（Actions）などを実装。
- documentsフォルダに以下の２点を追加。
  - ChatGPT_Dialogue_Systematization.html（AIとの協創 rapporti: ChatGPT対話分析レポート）
  - remote_pc_switch_report.html（パソコンリモート起動スイッチ(仮) 企画レポート）

## 💡 使い方

### ドキュメントの追加方法

1. `documents/`フォルダにHTMLファイルをアップロード
2. HTMLファイルには必ず`<title>`タグを設定
   ```html
   <title>ドキュメントのタイトル</title>
   <meta name="description" content="概要説明">
   <meta name="author" content="作成者名">
   ```
3. GitHub Actionsが自動的にメタデータを抽出
4. ページに自動反映（数分かかる場合があります）

### ファイル命名規則

- **ファイル名**: 英数字とアンダースコア/ハイフンを使用
- **例**: `project_proposal_2025.html`
- URL共有時の可読性を考慮して日本語は避ける

## 🛠️ 技術スタック

- **フロントエンド**: Vanilla JavaScript + HTML/CSS
- **ホスティング**: GitHub Pages
- **CI/CD**: GitHub Actions
- **メタデータ処理**: Node.js + Cheerio

## 📄 ライセンス

個人利用のプロジェクトです。

## ✉️ コンタクト

Ryo Tamura
ryo.tamura.ite@gmail.com

---

*Last updated: 2025/09/07*
