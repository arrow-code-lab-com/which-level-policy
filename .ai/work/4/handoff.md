---
issue: 4
flow: ai-default-medium
status: impl-success
outcome: "実装完了"
evidence:
  spec_status: none
  has_issue: true
  has_pr: false
  tasks_total: 0
  tasks_done: 0
  integration: none
  open_major: 1
  merged: false
  accepted: false
passed: [impl]
attempts: { impl: 1 }
edges:
  impl->review: 2
  review->impl: 1
events: 25
---

# Issue #4 の索引

この索引は `events/` から機械的に生成される写しです。手で書き換えないでください（次の記録で上書きされます）。

- 現在地: `impl-success`（outcome: 実装完了）
- フロー: `ai-default-medium` / 通過: `impl`
- open な指摘: 1 件（Major 以上 1 件）

## open な指摘

- Major `.ai/work/4/events` 受入条件「Google Maps についての記述がポリシーと利用規約に入っている」に kind: verification の event が無い … `events/20261110T110115-review.yaml`

## 直近の経路

- impl → review
- review ↩ impl（Major 2 件: iOS にはアプリ単体のキャッシュ消去が無いのにそれで消せると書いている／受入条件の verification の記録が無い）
- impl → review

## 記録（判断・懸念・検証・環境・質問）

- env [impl] ビルド・テストの手段がリポジトリに無い（静的 HTML のみ。README に記載なし）。代わりに index.html・terms.html のタグの入れ子を検査して通した … `events/20261110T105915-impl.yaml`
- concern [impl] Issue のうち人の作業は未対応: ポリシーの公開 URL（GitHub Pages）とサポート窓口の URL・メールの用意。また which-level#25（料金看板の OCR と AI で料金を試算）がポリシーに未反映の可能性があるが、#4 の範囲外のため触っていない … `events/20261110T105916-impl.yaml`
- verification [impl] 受入条件「Google Maps についての記述がポリシーと利用規約に入っている」: which-level docs/privacy/google-maps.md と突き合わせた。§1 送信 3 項目（表示範囲・端末とアプリの情報・API キー）→ index.html 第 4 章 (1) 日英に有り（IP アドレスも追記）。§2 利用規約の追加利用規約 → terms.html 第 6 条 日英に有り（terms_maps へのリンク）、ポリシーの Google プライバシーポリシー参照 → index.html 第 4 章 (1) と terms.html 第 6 条に有り。§4 キャッシュ（SDK が保存・全データ削除で消えない・アプリ削除で消える）→ index.html 第 2・5・7 章 日英に有り。OSM の記述は 3 ページとも 0 件。公開 URL とサポート窓口は人の作業で未完（concern 記録済み） … `events/20261110T110416-impl.yaml`
