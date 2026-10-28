# memory/のアーカイブ・整理（トークン消費対策）

`memory/task-log.md`・`memory/feedback-log.md`・`memory/learnings.md`は追記し続ける設計のため、放置すると肥大化し、
毎回のタスクで読み込む際のトークン消費が無駄に増えていく。これを防ぐため、定期的に「生ログを要約してアーカイブへ退避し、学びのエッセンスだけ残す」整理を行う。

tech-research-trackingスキルの「正本を更新し、古い版は`99_アーカイブ/`へ退避する」という考え方をmemory/にも適用したもの。

## このスキルが発動する条件
- 「メモリを整理して」「task-log.mdが長くなってきた」「アーカイブして」
- 四半期ごとの定期実行（schedule/loopスキル経由）
- 本人からの明示的な指摘がなくても、`memory/task-log.md`・`memory/feedback-log.md`の行数がそれぞれ**150行を超えたタイミング**で、次にmemory/を触るタスクの際に本人に整理を提案する

## 進め方
1. **対象ファイルを読む**：`memory/task-log.md`・`memory/feedback-log.md`を全文読む
2. **残す範囲を決める**：直近1〜2ヶ月分（または直近20〜30件）はそのまま残す。それより古い分をアーカイブ対象とする
3. **学びのエッセンスをlearnings.mdに残す**：アーカイブ対象の記録のうち、今後も参照する価値がある学び・パターンは、`memory/learnings.md`に要約して残す（生ログそのものではなく、エッセンスのみ）
4. **古い記録をアーカイブへ退避する**
   - 保存先：`memory/archive/task-log-YYYY-QN.md`、`memory/archive/feedback-log-YYYY-QN.md`（四半期単位。例：`task-log-2026-Q4.md`）
   - 元のtask-log.md・feedback-log.mdからは該当行を削除し、ファイル冒頭に「過去の記録は`memory/archive/`を参照」という一文を残す
5. **整理した記録をtask-log.mdに1行追記する**（整理作業自体も通常のタスクとして記録する。例：「2026-XX-XX | memory整理 | task-log.md/feedback-log.mdの2026-XX〜XX分をarchive/へ退避、学びをlearnings.mdに集約」）

## 品質基準
- アーカイブする際、生ログは消さずに必ず`memory/archive/`へ移す（削除しない）
- 学びのエッセンスは「何が起きたか」ではなく「次に活かせる教訓・パターン」の形で書く（tech-research-trackingの情報信頼度ラベルや、feedback-log.mdの「学び」欄の書き方を踏襲する）
- 直近の記録（1〜2ヶ月分）は常にtask-log.md・feedback-log.md本体に残し、すぐに参照できる状態を保つ
- soul/・knowledge/・skills/配下のファイルはこのスキルの対象外（これらは参照頻度が高く、肥大化のペースも緩やかなため）

## 自動化の進め方（運用メモ）
- 最初は本人からの声かけ、またはファイル行数が閾値を超えた際の提案ベースで実行する
- 四半期ごとの定期実行に移行する場合は、`schedule`スキルまたは`loop`スキルで設定する（本人の確認を得てから設定する）
