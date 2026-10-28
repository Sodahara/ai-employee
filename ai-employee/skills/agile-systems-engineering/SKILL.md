# アジャイル×システムズエンジニアリング×上流要求分析（ハードテック・防衛領域）

CADやモジュラーデザインのような「設計の中間プロセス」ではなく、**上流（要求分析・システムアーキテクチャ・開発プロセス自体をどう進めるか）** に焦点を当てたスキル。
ハードテック・防衛重工クライアント向けに、「アジャイルはソフトウェア起源の手法だが、ハードウェア・防衛システムにどう適応させるか」という最先端の知見を蓄積・活用する。

[frontier-knowledge-scouting](../frontier-knowledge-scouting/SKILL.md)の2026-10-28実行回でリサーチし、本人の承認を得て反映。

## このスキルが発動する条件
- 「アジャイル」「アジャイル開発」「スクラム」「SAFe」をハードウェア・防衛システム開発の文脈で検討する場合
- 「要求分析」「要求工学」「システムズエンジニアリング」「MBSE」が絡み、特に不確実性・変化対応力の観点が必要な場合
- クライアント（防衛重工等）への「アジャイル導入は可能か」「海外の防衛産業はどうしているか」という相談

## 最先端プレイヤー（継続ウォッチ対象）
| 人物・団体 | 立場 | 要点 |
|---|---|---|
| **Rick Dove** | INCOSE Fellow、Agile Systems & SE Working Group 議長、著書『Response Ability』 | アジャイルシステムズエンジニアリングの理論的第一人者。「応答要件」フレームワークの提唱者 |
| **Suzette Johnson** | Northrop Grumman Fellow（Lean-Agile）、Space Systems部門、NDIA Systems Engineering Division共同議長 | 防衛・航空宇宙の現場実務家。90,000人規模のLean-Agile変革を主導。著書『Industrial DevOps』 |
| **INCOSE Agile Systems & SE Working Group** | Dove（議長）＋Larri A. Rosser, Robin J. Yeman, Ron H. Lyells（共同議長） | 「アジリティはシステムアーキテクチャに規定・制約される能力」という立場でFuSE Agilityロードマップ（9つの基礎概念）を構築中 |
| Ali Hajou & Marina Voropaeva | 著書『Engineering Agility』 | SAFe・Scrumのハードウェア開発への実践的適応ガイド |

## 知見ベース

### 1. Rick Doveの「応答要件（Response Requirements）」フレームワーク
- 出典：[INCOSE Agile 105 - Operational Awareness](https://www.incose.org/docs/default-source/enchantment/160914-doverick-agile105-operationalawareness-slidesupdated.pdf)、著書『Response Ability』
- 要求を以下の2系統・8分類で整理する：
  - **反応型（Reactive）**：修正（Correction）／変動（Variation）／拡張（Expansion）／再構成（Reconfiguration）
  - **先行型（Proactive）**：創造（Creation）／改善（Improvement）／移行（Migration）／改変（Modification）
  - 各要求を コスト・時間・品質・スコープ の4軸で応答性能として評価する
- **使い方**：クライアントの要求分析時、従来の静的な要求定義表（「〇〇ができること」）に加えて、「この要求は将来どう変化しうるか、その変化にどう応答すべき要求か」という軸を一行追加する。不確実性が高いハードテック事業で特に有効
- 関連：静的な**アーキテクチャ**（設計工学の構造面）がアジリティの能力を規定し、動的な**ConOps（運用構想）**がその振る舞いを統制する、という二層構造で捉える

### 2. Suzette Johnsonの「Industrial DevOps」
- 出典：著書『Industrial DevOps』、[NDIA Systems Engineering Division](https://ndia.org/events/2025/2/28/power-of-prototyping-symposium/speakers/suzette-johnson)
- Northrop Grumman Space Systems部門での実践知。ソフトウェア起源のLean/Agile/DevOpsを、ハードウェアを含む複雑なサイバーフィジカルシステム開発に拡張
- **使い方**：防衛重工クライアントへの提案時、「海外の防衛産業（Northrop Grumman等）がどうアジャイル移行を進めているか」の具体的なベンチマーク・引用元として使う。「アジャイルはソフトウェアだけのもの」という反論への反証材料になる

### 3. アジャイル×要求工学×MBSEの統合はまだ発展途上（過信注意）
- 出典：[Rüttger, Albrecht, Toledo Gandarias (2026)](https://www.sciencedirect.com/science/article/pii/S1877050926007842)
- サイバーフィジカルシステムにおける「アジャイルのスケーリング戦略」「要求工学」「モデルベースシステムズエンジニアリング（MBSE）」の統合は、研究としてもまだギャップが指摘されている段階
- **使い方**：クライアントに提案する際、「成熟した確立手法」としてではなく「先進事例はあるが発展途上の領域」として適切な期待値設定をする

### 4. 『Engineering Agility』（SAFe・Scrumのハードウェア適応）
- 出典：Ali Hajou & Marina Voropaeva, [Scaled Agile Frameworkブログ](https://framework.scaledagile.com/blog/new-book-on-agile-hardware-development-engineering-agility)
- ソフトウェア向けに作られたSAFe・Scrumを、ハードウェア開発の制約（長い物理試作サイクル、規制対応、変更コストの非対称性）に適応させる実践パターン集
- **使い方**：「アジャイルを導入したいがハードウェアだから無理」という悩みへの、具体的な適応パターンの参照先

## 品質基準・注意点
- アジャイル×ハードウェアはまだ発展途上の領域であることを常に明示する（過度に成熟した手法として売り込まない）
- 防衛・航空宇宙という業界の近さ（Suzette Johnson等）を優先的に引用する。ソフトウェア業界一般のアジャイル論をそのまま持ち込まない
- CAD・モジュラーデザインのような設計の中間プロセスは対象外（→別スキル）。本スキルは上流（要求分析・開発プロセス・アーキテクチャの統制原理）に専念する

## 継続ウォッチの進め方
- Rick Dove（INCOSE Agile Systems & SE WG）、Suzette Johnson（Northrop Grumman／NDIA）の新しい発表・著作・カンファレンス講演を定期的に確認する
- 確認先：INCOSE Agile Systems & SE Working Groupページ、NDIA Systems Engineering Division、Agile Alliance・SAFeコミュニティのカンファレンス発表
- 新しい知見が見つかったら、本ファイルの「知見ベース」に追記し、`memory/task-log.md`に記録する
- 頻度・実行形態（手動／schedule・loopでの定期実行）は本人の確認を得てから決める
