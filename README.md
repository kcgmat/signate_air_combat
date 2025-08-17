# signate_air_combat
signate 第4回空戦AIチャレンジ用のリポジトリです。
このリポジトリは、コンペティション参加のためのコードを管理しています。  
**注意: データセットは規約により再配布禁止のため、このリポジトリには含まれていません。**

---

## 📂 ディレクトリ構成
project/
├── agents/              # 自作エージェントの実装
│   ├── base_agent.py    # ベースクラス（共通処理）
│   ├── rule_based.py    # ルールベース型
│   ├── rl_agent.py      # 強化学習型
│   └── __init__.py
│
├── sim/                 # 提供されたシミュレータコード
│   ├── core/            # 公式のシミュレータ（改変禁止部分）
│   ├── wrapper/         # 環境のラッパークラス（観測加工など）
│   └── README.md
│
├── training/            # 学習・評価関連
│   ├── train.py         # 学習用スクリプト
│   ├── evaluate.py      # 評価スクリプト（対戦シミュレーション）
│   └── replay/          # ログ・リプレイ保存
│
├── notebooks/           # EDA・実験用ノートブック
│   ├── env_check.ipynb
│   └── reward_tuning.ipynb
│
├── utils/               # 補助関数（ログ、可視化、データ処理など）
│   ├── logger.py
│   ├── plot.py
│   └── config.py
│
├── configs/             # パラメータやハイパーパラメータ設定
│   ├── agent_config.yaml
│   └── train_config.yaml
│
├── tests/               # 動作確認用ユニットテスト
│   └── test_agent.py
│
├── data/                # （.gitignore で除外）提供データや生成データ
│
├── models/              # （.gitignore で除外）学習済みモデル
│
├── requirements.txt     # Python依存ライブラリ
├── run.sh               # 学習や評価のワンコマンド実行用
├── .gitignore           # データ/モデル/ログを除外
└── README.md            # プロジェクトの説明
