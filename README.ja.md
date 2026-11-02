# FlashNote - ひらめきの流光を、美しい章へと紡ぐ。

> **書くことだけに集中し、残りはすべてお任せください。**
> サイドバーで楽しむMarkdown集中ライティング、直感的なWYSIWYG、チャートや数式も自由自在。静的ブログへのワンクリック投稿から、執筆コンテンツのコラム化・電子書籍化まで。ひらめきの流光を、美しい章へと紡ぎます。

[![Release](https://img.shields.io/github/v/release/Aicrosoft/FlashNote?color=blue&label=Latest%20Release)](https://github.com/Aicrosoft/FlashNote/releases)
[![Help Documentation](https://img.shields.io/badge/Docs-%E3%83%89%E3%82%AD%E3%83%A5%E3%83%A1%E3%83%B3%E3%83%88-brightgreen)](https://aicrosoft.com/apps/flashnote/help/)
[![License](https://img.shields.io/badge/License-Proprietary-orange)](https://aicrosoft.com/)

📖 **公式オンラインドキュメント**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)  
💬 **問題報告＆フィードバック**: [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues)

**対応言語 (Languages)**:  
[🇨🇳 简体中文](README.zh-CN.md) | [🇺🇸 English](README.en.md) | [🇭🇰 繁體中文](README.zh-TW.md) | [🇯🇵 日本語](README.ja.md)

---

> [!WARNING]
> ⚠️ **デスクトップ版の注意事項 (Experimental Preview)**：  
> FlashNote デスクトップ版（macOS / Windows / Linux）は、Tauri 2.0 クロスプラットフォーム基盤を採用した**実験的プレビュー版**です。ご利用中に不具合、クラッシュ、または使い勝手の改善要望などがございましたら、お気軽に [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) までフィードバックをお寄せください！

---

## 🚀 デスクトップ版ダウンロード (Downloads & Releases)

[GitHub Releases](https://github.com/Aicrosoft/FlashNote/releases) ページより、各OS向けの最新インストーラーをダウンロードいただけます：

| オペレーティングシステム | パッケージ形式 | 説明 |
| :--- | :--- | :--- |
| **macOS** | `.dmg` / `.app.zip` | Mac 用インストーラー / ポータブル Zip |
| **Windows** | `.exe` / `.msi` | NSIS セットアップウィザード / Windows インストーラー |
| **Linux** | `.AppImage` / `.deb` | ポータブル AppImage / Debian & Ubuntu パッケージ |

---

## 🌟 主な機能と特徴 (Feature Highlights)

### 1. ✍️ 純粋な没入型 Markdown ライティング
- **WYSIWYG エディター**：Tiptap (ProseMirror) モダンコアをベースに、コードハイライト、テーブル、リスト、タスク項目をリアルタイムレンダリング；
- **タイピング遅延の完全解消**：タイトル入力を内部のマイクロステートへ分離し、連続入力時の不要な再描画やディスク書き込みを抑止。Enter キーで本文ファースト行へスムーズ遷移；
- **貼り付けタイトルの自動整形**：外部からコピーしたタイトルから行頭の `#` や不要な装飾記号を自動除去；
- **KaTeX 数式レンダリング**：行列 (Matrix) や連立方程式 (Cases)、高階積分数式を美しく忠実に表示。

### 2. 🌐 高機能Webクリッパー＆オフライン保存
- **フォーラム全レスの一括取得**：技術系掲示板（Discourse / LINUX DO など）に深く対応。クリッパーをクリックするだけで、表示中の親記事とすべての返信スレッド（`### #1 投稿者`、`### #2 返信`...）を整然とノートへ取り込み；
- **文字数制限なしの右クリック深層要約**：右クリック「Webページを要約」の文字数上限を撤廃。見出し構造、コードブロック、高解像度画像を維持しつつ、ノイズコメントを自動除去；
- **Web画像の自動オフライン保存**：記事保存時にバックグラウンドで画像の一括オフライン同期が走り、外部サイトの画像削除や直リンク禁止（Hotlinking）によるリンク切れを防止。

### 3. 🛡️ 誤削除防止の安心設計＆Notion風プロパティバー
- **誤操作を防ぐ安全なUI**：同名ノートの整理ダイアログにおいて「選択中ノートのみをゴミ箱へ移動」を目立つ既定ボタンとし、他の同名ノートを100%保護。「すべてゴミ箱へ移動」も5秒間の取り消し通知で瞬時に復旧可能；
- **メタデータのスマート配置**：フォルダやタグの選択を横並びに集約。末尾には直感的な「電子書籍・コラム化」トリガーを配置；
- **集中を妨げないブリージングステータスバー**：不要なタイトル表示を省き、リアルタイム文字数、保存ステータス、ネットワーク状態に特化したミニマルな呼吸インジケーターを採用。

### 4. ☁️ クラウド同期の安定化＆Gitブログワンクリック公開
- **大容量ファイル 4MB 分割ストリーミング同期**：長編書籍や添付ファイルを4MB境界で自動スライスし、Precreate MD5検証と最終結合を実行してタイムアウトを根絶；
- **ステートマシンの中断自己修復**：通信途絶時も安全にロールバックし、レジューム機能でOPFSローカルサンドボックスとクラウドの整合性を保証；
- **英名スラッグの重複自動解消**：同名ノートに連番（例: `ebookunpack-2`）を自動付与して衝突を回避。日常メモでは不要なAI翻訳を実行せずクォータを保護；
- **Git 連携による静的ブログへの直接公開**：作成した記事をワンクリックで GitHub や Azure DevOps リポジトリへプッシュし、公開ライフサイクルを可視化。

### 5. 📚 コラム連載の電子書籍（EPUB 3.0）書き出し
- **ノートの書籍化**：書き溜めたノートを章立て構成して1冊の本にまとめ上げ；
- **EPUB 3.0 / Markdown パッケージ**：本格的な表紙デザインプリセットを備え、各種電子書籍リーダーでそのまま読める形式で書き出し；
- **完全クライアントサイド PlantUML $\to$ Mermaid 自動変換**：外部サーバー不要でブラウザ内で高速変換。コードとプレビューの切り替え、SVG / 高解像度 PNG エクスポートに対応。

### 6. 🤖 AI長文アシスタントの進化
- **生成開始時のパネル自動格納**：生成実行と同時に調整パネルが自動で折りたたまれ、タイプライター風のストリーミング出力を広々と確認可能；
- **生成の中断操作を一本化**：生成中にパネルを再度開くと、ボタンが赤色の「■ 生成を停止」へ切り替わり、ワンクリックで停止可能；
- **エピック（5,000字以上）＆レジェンダリー（8,000字以上）対応**：構成案から本文まで多階層に長文を構築。自然、技術的、ビジネス、文学的など6種類の文体をサポート。

---

## 💬 サポート＆フィードバック

- 📖 **公式オンラインドキュメント**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)
- 🐞 **不具合報告・ご要望**: [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) よりお気軽にお寄せください。
