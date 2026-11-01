# FileListRetrievalTool_VBA
Excel VBA ファイル一覧取得ツール（v1.0）

## ツール概要
Excel VBAで作成したファイル一覧取得ツールです。
指定したフォルダ内のファイル情報を一覧化し、 FileListシートへ出力します。
サブフォルダを含めた検索や、 拡張子によるフィルタリングに対応しています。

## 開発環境
・Microsoft Excel
・Excel VBA

## 主な機能
・FileDialogによるフォルダ選択
・ファイル一覧取得
・サブフォルダ再帰探索
・拡張子フィルタリング

## 画面イメージ・操作手順
### ① Settings画面
<img src=① Settings画面.png width="400">

### ② フォルダ選択(FileDialog)
<img src=② フォルダ選択(FileDialog).png width="400">

### ③ 出力完了メッセージ
<img src=③ 出力完了メッセージ.png width="400">

### ④ FileList出力結果
<img src=④ FileList出力結果.png width="400">

## コード抜粋
<img src=Code抜粋.png width="400">

## 工夫したポイント
・シート存在チェックを実装し、必要シート不足時は処理を中断
・フォルダ有効性確認を実装し、不正なパス指定を防止
・再帰処理によるサブフォルダ探索に対応
・Dictionaryを利用した拡張子フィルタリング
・入力値チェックにより異常系を考慮

## テスト
単体テストを実施しました。
・正常系：各機能の動作確認
・異常系：PATH未指定、不正入力、対象シートなし等
全テスト項目で期待結果を確認済みです。

## フォルダ構成
docs/
├─要件定義.docx
├─設計書.docx
├─詳細設計書.docx
├─テスト仕様書.xlsx
└─バージョン管理メモ.txt

images/
├─①Settings画面.png
├─②フォルダ選択(FileDialog).png
├─③出力完了メッセージ.png
├─④FileList出力結果.png
└─Code抜粋.png

README.md

## ドキュメント
・要件定義
・設計書
・詳細設計書
・テスト仕様書
・バージョン管理メモ

---

## License
このリポジトリは GNU GPL v3.0 ライセンスのもとで公開しています。
