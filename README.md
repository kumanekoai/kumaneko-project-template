# kumaneko-project-template

くまねこAIプロジェクト用のスタータテンプレートです。

## 含まれているもの

- `.gitignore` — Next.js + Cloud Run プロジェクト用の標準設定（秘密情報保護含む）
- `.github/workflows/gitleaks.yml` — 秘密情報漏洩検知のCI（無料・gitleaks CLI）
- `.gitleaksignore` — 誤検知を登録するファイル（空）

## 使い方

### 新規プロジェクトを作成するとき

1. GitHubでこのリポジトリを開く
2. 緑の **「Use this template」** ボタンをクリック
3. 「Create a new repository」を選択
4. リポジトリ名を入力して作成

新しいリポジトリは最初から上記ファイル一式が入った状態で始まります。

### 個人アカウントでも使える

このリポジトリは Public なので、個人アカウントでの新規プロジェクトにも `Use this template` から使えます。

## なぜ用意しているか

過去に `env-cloudrun.yaml`（SP-API認証情報入り）が誤ってgitにコミットされた事故がありました。
原因は初期の `.gitignore` が `.env*` しか除外していなかったこと。

このテンプレートから派生させれば、そういった事故を最初から防げます。

## 詳細ドキュメント

- [kumaneko-ops/templates/gitignore-nextjs.md](https://github.com/kumanekoai/kumaneko-ops/blob/main/templates/gitignore-nextjs.md)
- [kumaneko-ops/templates/gitleaks-setup.md](https://github.com/kumanekoai/kumaneko-ops/blob/main/templates/gitleaks-setup.md)
