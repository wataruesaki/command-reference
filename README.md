# コマンドリファレンス

## Table of contents

・[git](#git)

・[npm](#npm)

・[yarn](#yarn)

## git

### 初期化

```zsh
git init
```

### ログを表示

```zsh
git log
```

### ステータスを表示

```zsh
git status
```

### ブランチ間の差分を表示

Bが最新のブランチであると仮定して差分を表示します。

```zsh
git diff A..B
```

### カレントブランチとリモートのmainブランチの差分を表示

プル前に実行すると便利です。

```zsh
git diff HEAD..origin/main
```

### リモートのmainブランチとカレントブランチの差分を表示

プッシュ前に実行すると便利です。

```zsh
git diff origin/main..HEAD
```

### フェッチ

```zsh
git fetch origin [branch]
```

### カレントブランチにマージ

```zsh
git merge origin [branch]
```

### カレントブランチにプル

```zsh
git pull origin [branch]
```

### mainブランチを更新

```zsh
git checkout main && git pull origin HEAD
```

### ブランチの一覧を表示

```zsh
git branch
```

### カレントブランチから派生するブランチを作成し移動

```zsh
git checkout -b [branch]
```

### ブランチ名を変更

```zsh
git branch -m [branch]
```

### ブランチを削除

```zsh
git branch -d [branch]
```

### ステージングしていない変更の差分を表示

```zsh
git diff
```

### ステージングしていない特定の変更の差分を表示

```zsh
git diff -- [path]
```

### ステージングした変更の差分を表示

```zsh
git diff --cached
```

### ステージングした特定の変更の差分を表示

```zsh
git diff -- [path] --cached
```

### 変更をステージング

```zsh
git add .
```

### 特定の変更をステージング

```zsh
git add -- [path]
```

### 変更のステージングを取り消す

```zsh
git reset
```

### 特定の変更のステージングを取り消す

```zsh
git reset -- [path]
```

### カレントブランチでコミットしていない変更を取り消す

```zsh
git checkout .
```

### コミット

```zsh
git commit -m [comment]
```

### 1つ前のコミットメッセージを修正

```zsh
git commit --amend -m [comment]
```

### 初回のプッシュ

```zsh
git push -u origin HEAD
```

### 2回目以降のプッシュ

```zsh
git push origin HEAD
```

### 変更を避難

```zsh
git stash
```

### 避難した変更の一覧を表示

```zsh
git stash list
```

### 避難した変更を呼び出す

```zsh
git stash apply
```

### 避難した変更を削除

```zsh
git stash clear
```

## npm

## yarn
