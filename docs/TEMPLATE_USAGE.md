# テンプレートリポジトリの使い方

## 新しいプロジェクトを開始する

### 1. このテンプレートから新しいリポジトリを作成

1.[project-template](https://github.com/jun-learning/project-template) に移動
2.「Use this template」→「Create a new repository」をクリック
3.新しいリポジトリ名を入力（例：flask-todo-mysql）
4.「Create repository」

### 2. リポジトリをクローン

    ```bash
    git clone git@github.com:jun-learning/NEW_REPO_NAME.git
    cd NEW_REPO_NAME
    ```

### 3. git-flow初期化

    ```bash
    git flow init -d
    ```

### 4. README.mdを編集

プロジェクト固有の情報に更新してください：
-プロジェクト名
-説明
-技術スタック
-環境構築手順

### 5. 開発開始

    ```bash
    # 最初の機能開発
    git flow feature start initial-setup
    ```

## Issueの作成方法

1.リポジトリ →「Issues」→「New issue」
2.テンプレートを選択（バグ報告 or 機能リクエスト）
3.必要事項を記入
4.「Submit new issue」

## Pull Requestの作成方法

1.featureブランチで開発
2.コミット & プッシュ
3.GitHubで「Compare & pull request」
4.テンプレートに従って記入
5.「Create pull request」

## ブランチ保護について

-mainブランチへの直接pushは禁止
-developブランチへの直接pushは禁止
-Pull Requestを経由してマージ
-CI/CDチェックが必須