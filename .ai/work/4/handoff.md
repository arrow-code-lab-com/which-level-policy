---
issue: 4
flow: ai-default-medium
status: review-revert
outcome: findings
evidence:
  spec_status: none
  has_issue: true
  has_pr: false
  tasks_total: 0
  tasks_done: 0
  integration: none
  open_major: 2
  merged: false
  accepted: false
passed: [impl]
attempts: {}
edges:
  impl->review: 1
  review->impl: 1
events: 16
---

# Issue #4 の索引

この索引は `events/` から機械的に生成される写しです。手で書き換えないでください（次の記録で上書きされます）。

- 現在地: `review-revert`（outcome: findings）
- フロー: `ai-default-medium` / 通過: `impl`
- open な指摘: 7 件（Major 以上 2 件）

## open な指摘

- Major `index.html:137` 地図のキャッシュの消し方「端末の設定から本アプリのキャッシュを消去」は iOS では行えない（日英とも） … `events/20261110T110114-review.yaml`
- Major `.ai/work/4/events` 受入条件「Google Maps についての記述がポリシーと利用規約に入っている」に kind: verification の event が無い … `events/20261110T110115-review.yaml`
- Minor `index.html:79` 地図（Google Maps）で送られる情報から IP アドレスが消えた（旧 OpenStreetMap の節には書いていた） … `events/20261110T110116-review.yaml`
- Minor `index.html:70` Android の権限の注記が「広告・課金の SDK」だけで、新たに入った Google Maps SDK が足す権限に触れていない … `events/20261110T110244-review.yaml`
- Minor `index.html:76` 「地図を表示するたびに…送信されます」が、同じ文書の地図のキャッシュの記述と食い違う … `events/20261110T110245-review.yaml`
- Minor `index.html:137` 「本アプリからは削除できない」がアプリの実際の動作（全データ消去がキャッシュのディレクトリを消すか）と一致しているか未確認 … `events/20261110T110246-review.yaml`
- Minor `index.html:35` 冒頭の「施行日: 2026年11月5日（初版）」のままで、改定版の施行日と改定の告知が無い … `events/20261110T110247-review.yaml`

## 直近の経路

- impl → review
- review ↩ impl（Major 2 件: iOS にはアプリ単体のキャッシュ消去が無いのにそれで消せると書いている／受入条件の verification の記録が無い）

## 記録（判断・懸念・検証・環境・質問）

- env [impl] ビルド・テストの手段がリポジトリに無い（静的 HTML のみ。README に記載なし）。代わりに index.html・terms.html のタグの入れ子を検査して通した … `events/20261110T105915-impl.yaml`
- concern [impl] Issue のうち人の作業は未対応: ポリシーの公開 URL（GitHub Pages）とサポート窓口の URL・メールの用意。また which-level#25（料金看板の OCR と AI で料金を試算）がポリシーに未反映の可能性があるが、#4 の範囲外のため触っていない … `events/20261110T105916-impl.yaml`
