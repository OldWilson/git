# 撤销

## git reset

### 1. 原理
### 2. git reset
* git reset HEAD^ / git reset HEAD~1 上一次提交
* git reset HEAD^^ / git reset HEAD^2 倒数第三次
* git reset HEAD^^^ / git reset HEAD^3 倒数第四次
### 3. 区别
* git reset -mixed （默认方式）
  会将暂存区的内容和本地已提交的内容全部恢复到未暂存的状态，不影响原来本地文件（未提交的不受影响）
* git reset -soft
  不清空暂存区，将已提交的内容恢复到暂存区，不影响原来本地的文件（未提交的不受影响）
* git reset -hard
  清空暂存区，将已提交的内容的版本恢复到本地，本地的文件也将被恢复的版本替换

git push origint <分支名> --force