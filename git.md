# Git
### clone + 重新命名
```git
$ git clone https://github.com/name/repository.git   [yournewname]
```
### 改變最後一次提交
```git
$ git commit --amend
```
### git reset HEAD^ 
放棄之前的commit 將HEAD指回去 ，`^`代表次數
    * `--soft` staged、worktree 不更動
    * `--mixed` (預設) staged還原, worktree 不更動 
    * `--hard` 全部還原
### 變更https或SSH
1. 
```git
$ git git remote -v
origin  https://github.com/USERNAME/REPOSITORY.git (fetch)
origin  https://github.com/USERNAME/REPOSITORY.git (push)
```
2. 
```git
$ git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
```
