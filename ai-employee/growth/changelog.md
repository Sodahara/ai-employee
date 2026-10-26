# 成長の変更履歴

<!-- AI社員の成長を時系列で記録する -->

## 2026-03-25 - 初期セットアップ
- フォルダ構成を作成
- 各レイヤーのテンプレートファイルを配置
- CLAUDE.md（エントリポイント）を作成

## 2026-10-26 - 記憶蓄積・週次レビューの動作確認（Day4-5）
- サンプルタスク（事業構造サマリー）を実行し、memory/task-log.mdへの自動記録を確認
- growth/weekly-review/2026-W44.mdで模擬週次レビューを実施
- knowledge/company.mdを職務経歴書に基づき更新（事業内容・クライアント・提供価値を反映）

## 2026-10-26 - 模擬週次レビュー承認
- growth/weekly-review/2026-W44.mdの内容をオーナーが承認
- 今回は提案事項なし（スキル追加・ルール変更なし）。成長ループ（実行→記録→レビュー→承認）が一巡したことを確認

## 2026-10-26 - 本業スキルを追加
- skills/technical-pm/SKILL.md（技術PM資料作成：WBS・開発Gate・課題管理）を新規追加
- skills/design-knowledge-doc/SKILL.md（設計ノウハウ・暗黙知のドキュメント化）を新規追加。日本語執筆はjapanese-writing-techniqueスキル参照を必須化
- skills/_registry.mdを更新（4スキル→6スキル）

## 2026-10-26 - 本業スキルを4件追加
- skills/certification-safety-management/SKILL.md（認証・安全対応管理）
- skills/business-strategy-research/SKILL.md（事業戦略・新規参入検討リサーチ）
- skills/cost-planning-lcc/SKILL.md（原価企画・ライフサイクルコスト分析）
- skills/stakeholder-alignment/SKILL.md（ステークホルダー調整・合意形成）
- skills/_registry.mdを更新（6スキル→10スキル）。要求定義系タスクは既存のrequirements-engineeringスキルを流用する方針を明記

## 2026-10-26 - スキルをウェブ上の権威ある情報源でブラッシュアップ
- 技術PM資料作成: Stage-Gate法（Robert G. Cooper）のGate判定基準の考え方を追加
- 認証・安全対応管理: 船級協会の認証ステップ（AiP/GDA/Technology Qualification）、IACSの枠組みを追加
- 事業戦略・新規参入検討リサーチ: TAM/SAM/SOM、3C分析、事業性評価の考え方を追加
- 原価企画・ライフサイクルコスト分析: 原価企画（ターゲットコスティング）、VE（SAVE International Value Methodology）、LCC（IEC 60300-3-3）を追加
- ステークホルダー調整・合意形成: PMBOK（PMI）のステークホルダー・マネジメントプロセス、Power-Interest Gridを追加
- 設計ノウハウ・暗黙知のドキュメント化: SECIモデル（野中郁次郎・竹内弘高）の「外化」工程として位置づけを追加
- いずれも一次情報（規格・学会発行の標準等）に当たれなかった項目は、その旨を注記
