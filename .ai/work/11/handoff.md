---
issue: 11
pr: 12
flow: ai-default-medium
status: pr-success
outcome: ready
evidence:
  spec_status: agreed
  has_issue: true
  has_pr: true
  tasks_total: 0
  tasks_done: 0
  integration: none
  open_major: 0
  merged: false
  accepted: false
passed: [triage, impl, review, pr]
attempts: {}
edges:
  triage->impl: 1
  impl->review: 1
  review->pr: 1
  pr->done: 1
artifacts:
  triage:
    - .ai/specs/spec-20261117-074954.md
events: 19
---

# Issue #11 の索引

この索引は `events/` から機械的に生成される写しです。手で書き換えないでください（次の記録で上書きされます）。

- 現在地: `pr-success`（outcome: ready）
- フロー: `ai-default-medium` / 通過: `triage` → `impl` → `review` → `pr`
- open な指摘: 3 件（Major 以上 0 件）

## open な指摘

- Minor `.ai/work/11/events` impl が decision / concern を 1 件も積んでいない（何を直し何を残したかの判断が events に無い） … `events/20261116T225242-review.yaml`
- Minor `.ai/specs/spec-20261117-074954.md:28` spec のゴール（全公開ページを読み問題を直す）に対し、PR は deploy のコピー対象に app.html を足しただけ … `events/20261116T225358-review.yaml`
- Minor `.github/workflows/deploy.yml:25` 手で保つ許可リストに 1 語足す対症療法で、ページ追加時に載せ忘れる構造は残る … `events/20261116T225359-review.yaml`

## 成果物

- triage: `.ai/specs/spec-20261117-074954.md`

## 直近の経路

- triage → impl
- impl → review
- review → pr
- pr → done

## 記録（判断・懸念・検証・環境・質問）

- concern [review] Android は描画前に必ず Play Store へ飛ばされ、app.html のリンクを読めない … `events/20261116T225410-review.yaml`
- concern [review] APP_STORE_ID 設定後は iOS も無条件リダイレクトで履歴から page が消える … `events/20261116T225411-review.yaml`
- concern [review] APP_STORE_ID を形式チェックなしで連結している … `events/20261116T225412-review.yaml`
- concern [review] Play Store の URL が 3 か所にハードコードされている … `events/20261116T225413-review.yaml`
- concern [review] setLang が 4 ページに逐語コピーされている … `events/20261116T225414-review.yaml`
- concern [review] app.html のフッターに特定商取引法に基づく表記へのリンクが無い … `events/20261116T225415-review.yaml`
- concern [review] プライバシーポリシーの公開ページ・関連文書の一覧に app.html が無い … `events/20261116T225416-review.yaml`
