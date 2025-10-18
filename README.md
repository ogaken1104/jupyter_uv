# uvを用いたjupyter notebook開発のミニマム環境
## 概要
- uvを用いた環境での開発を行うためのミニマムなテンプレート
- ``uv sync``で依存関係をインストール後使用可能となる

## 動作確認環境
- macOS Sequoia 15.3.2

## the structure of the repository

```
.
├── README.md                 # プロジェクトの説明文書
├── pyproject.toml           # Python プロジェクトの設定ファイル（依存関係、ビルド設定等）
├── uv.lock                  # uv による依存関係のロックファイル
├── .python-version          # 使用する Python バージョンの指定
├── .gitignore              # Git で追跡しないファイルの指定
├── notebooks/              # Jupyter Notebook ファイル格納ディレクトリ
│   └── example.ipynb       # サンプルノートブック
└── src/                    # Python ソースコード格納ディレクトリ
    └── __init__.py         # パッケージ初期化ファイル
```

## 本リポジトリの作成方法
- uv initを実行
- .gitignoreを、gitignore.ioから生成したもので更新
- jupyter kerenlを追加``uv add --dev ipykernel``
- src,dataディレクトリ、template.ipynbを追加

