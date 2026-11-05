# トリミング君：Codex適用記録
確認日：2026-11-05（日本時間）。対象：ken-tak-steam/trimming-kun の取得時の既定ブランチ。アプリ本体の改修・実機テストは今回実施していない。

## 確認した現状
READMEもCDN通信あり・完全オフラインではないと明記。コードでPDFをCanvasに描画し、jsPDF.addImageで出力しているため、元の文字・リンク保持とは扱えない。トリミング操作にmousedown/mousemove/mouseupを確認。iPadのタッチ対応は実機未確認。

## 本体ライセンス
LICENSE本文を確認。独自の非商用ライセンス。著作者・出典・改変表示を保持し、学校教育、有料・無料の講習会・研修会での教材利用を認める。MIT等ではない。

## 依存ライブラリ・付属データ
index.htmlでPDF.js 3.11.174、jsPDF 2.5.1、JSZip 3.10.1、FileSaver.js 2.0.5、Tailwind CDN、lucide@latestを確認。上流の該当タグでPDF.jsのApache-2.0、jsPDFのMIT、JSZipのMIT OR GPLv3を確認。JSZipの配布時にどちらを採用したかの明示と通知整備が必要。FileSaver、Tailwind、Lucideの取得物に対応する本文・固定バージョン、推移的依存は未確認。推測でライセンス名を埋めない。

## 次の適用順序
優先1：既存PDF読み込みを削除せず、ライブラリ・Worker・CSS・アイコンの固定と同梱を計画。優先2：Pointer Eventsとボタン操作の代替。優先3：画像出力と文字・リンクを保つPDF切り抜きを別扱いにし、互換性を検証。以前のPDF読み込み未対応オフライン試作で置き換えない。

## 取得根拠
- README.md: 519255204dcbaeec2773393d5d18f4e8e6263b03
- LICENSE: 6a4dcbc97767a4351487779347173ac80a05f5e2
- index.html: 8cc2e0208c572cf3761680af032f5d2ea58b7a50
ソース：https://github.com/ken-tak-steam/trimming-kun
取得したコードとREADMEの記述、過去チャットの報告は区別する。取得時点のファイル単位のSHAであり、リポジトリ全体の同一コミットを保証しない。

## 今回の変更範囲
AGENTS.mdとdocs/CODEX_APP.md、docs/CODEX_TEMPLATES.mdの追加のみ。既存HTML・ライセンス本文・依存バージョン・公開設定は変更しない。共通ルールは目標であり、現アプリが全条件を満たす証明ではない。
