+++
date = '2025-04-01T12:02:14+09:00'
draft = true
title = 'GitHub_memo'
+++
## Git/Githubの備忘録

### Local to Remote

```
GitHub上でリポジトリをあらかじめ作成しておくこと

cd <対象ディレクトリ>
git init # ローカルリポジトリの作成
git status # リポジトリの状態を確認
git add -A # ディレクトリ配下全てをステージングエリアに追加(コミットの予約)
git status
git commit -m "コミットの内容を入力"
git status

git branch -m <新しいブランチ名> # ブランチ名を変更する

git remote add <remote_repository_name> <remote_repository_URL>
	git remote add origin https://<user_name>:<access_token>@github.com/XX/XX.git
		# リモートブランチとの紐づけ

git push -u <repository_name> <local_branch_name>:<remote_branch_name>
	git push -u origin main
		# リモートブランチにアップロード(-u で上流ブランチを設定)->以降のpush,pullでブランチ名を指定しなくてよくなる
```
