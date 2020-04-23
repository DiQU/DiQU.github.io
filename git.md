# Git

## clone + 重新命名

```git
$ git clone https://github.com/name/repository.git   [yournewname]
```

## 改變最後一次提交

```git
$ git commit --amend
```

## git reset HEAD^

放棄之前的 commit 將 HEAD 指回去 ，`^`代表次數

- `--soft` staged、worktree 不更動
- `--mixed` (預設) staged 還原, worktree 不更動
- `--hard` 全部還原

## 變更 https 或 SSH

1. 查看 remote

```git
$ git remote -v

origin  https://github.com/USERNAME/REPOSITORY.git (fetch)

origin  https://github.com/USERNAME/REPOSITORY.git (push)
```

1. 設定成`SSH`連線

```git
$ git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
```

### 刪除遠端分支

#### 1.檢視遠端分支

`$ git branch -r`

#### 2.檢視本地分支

`$ git branch`

#### 3 刪除遠端分支

```git
$ git branch -r -d origin/branch-name

$ git push origin :branch-name
```
