# 開発ガイド

## 開発環境セットアップ

### 1. リポジトリクローン

    ```bash
    git clone git@github.com:jun-learning/project-name.git
    cd project-name
    ```

### 2. 環境変数設定

    ```bash
    cp .env.example .env
    # .env を編集
    ```

### 3. Docker起動

    ```bash
    docker compose up -d
    ```

## Git Flow運用

このプロジェクトはGit Flowを採用しています。

### 機能開発

    ```bash
    git flow feature start feature-name
    # 開発
    git flow feature finish feature-name
    ```

### リリース

    ```bash
    git flow release start x.x.x
    # バージョン更新
    git flow release finish x.x.x
    ```

## コーディング規約

-Python: PEP 8準拠、Black でフォーマット
-コミットメッセージ: Conventional Commits

## テスト

    ```bash
    # 全テスト実行
    pytest

    # カバレッジ測定
    pytest --cov=src --cov-report=html
    ```
