---
issue: 1
pr: 2
flow: ai-default-medium
status: review-revert
outcome: findings
evidence:
  spec_status: draft
  has_issue: true
  has_pr: true
  tasks_total: 0
  tasks_done: 0
  integration: none
  open_major: 3
  merged: false
  accepted: false
passed: [triage, requirements, impl]
attempts: {}
edges:
  triage->requirements: 1
  requirements->impl: 1
  impl->review: 1
  review->impl: 1
artifacts:
  triage:
    - .ai/specs/spec-20261105-004552.md
  requirements:
    - .ai/specs/spec-20261105-004552.md
    - .ai/specs/assets/20261105-004552/review.html
    - .ai/work/1/review.html
  impl:
    - index.html
    - terms.html
    - legal.html
events: 24
---

# Issue #1 の索引

この索引は `events/` から機械的に生成される写しです。手で書き換えないでください（次の記録で上書きされます）。

- 現在地: `review-revert`（outcome: findings）
- フロー: `ai-default-medium` / 通過: `triage` → `requirements` → `impl`
- open な指摘: 13 件（Major 以上 3 件）

## open な指摘

- Major `terms.html:45` iOS でもデータがバックアップされないと書いているが、iOS 版は iCloud／端末のバックアップと機種変更の移行の対象になる … `events/20261104T155952-review.yaml`
- Major `index.html:121` ML Kit が Google へ送る利用状況・性能の計測を書かず、分析目的の外部送信 SDK は無いと言い切っている … `events/20261104T160006-review.yaml`
- Major `.ai/specs/assets/20261105-004552/review.html:5` 追跡物の確認ページにローカルの絶対パス（ユーザー名を含む）が入っている … `events/20261104T160013-review.yaml`
- Minor `index.html:52` 設定項目「保存後すぐカメラを開く」を「自動撮影」と書いており、勝手に撮影するように読める … `events/20261104T160027-review.yaml`
- Minor `index.html:61` 第 3 章の権限一覧に、SDK のマージで入る Android の権限（AD_ID・BILLING 等）が無い … `events/20261104T160028-review.yaml`
- Minor `.ai/work/1/events` この Issue に kind: decision / concern の event が 0 件 … `events/20261104T160029-review.yaml`
- Minor `index.html:92` Android の広告 ID の送信を断定しており、spec U-2 の「利用する場合がある」と書く指示に沿っていない … `events/20261104T160204-review.yaml`
- Minor `index.html:109` UMP の同意前に広告を読まない・設定画面に「広告のプライバシー設定」があるという記載の裏付けが spec に無い … `events/20261104T160205-review.yaml`
- Minor `index.html:309` 言語の選択がページ移動・URL で保持されず、英語版を直接開く URL も無い … `events/20261104T160206-review.yaml`
- Minor `legal.html:49` 「購入を復元」の場所が特商法（設定画面）と利用規約（アプリ内）で書き方が違う … `events/20261104T160207-review.yaml`
- Minor `terms.html:88` 責任の上限が「広告なし版の支払額」なので、無料の利用者には全部免責になり消費者契約法 8 条 1 項で無効になり得る … `events/20261104T160208-review.yaml`
- Minor `legal.html:51` 動作環境に iPad を挙げているが spec では iPad 対応を確かめていない … `events/20261104T160209-review.yaml`
- Minor `index.html:308` setLang のスクリプトと style が 3 ページに重複している … `events/20261104T160210-review.yaml`

## 成果物

- triage: `.ai/specs/spec-20261105-004552.md`
- requirements: `.ai/specs/spec-20261105-004552.md`
- requirements: `.ai/specs/assets/20261105-004552/review.html`
- requirements: `.ai/work/1/review.html`
- impl: `index.html`
- impl: `terms.html`
- impl: `legal.html`

## 直近の経路

- triage → requirements
- requirements → impl
- impl → review
- review ↩ impl（Major 3件: iOSのバックアップ記載が実態と矛盾 / ML Kitの利用データ送信が未記載 / 追跡ファイルにローカル絶対パス）

## 記録（判断・懸念・検証・環境・質問）

- env [review] 事実確認用の which-level の作業ツリー（workspaces/which-level/画面修正）がレビュー途中で消えた … `events/20261104T160214-review.yaml`
