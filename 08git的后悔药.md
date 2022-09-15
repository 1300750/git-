### git的后悔药

工作区
  撤回工作区的修改
  git restore -- xxx
暂存区
  撤回暂存的操作
  git reset HEAD xxx
版本库
  撤回提交的版本
  git commit --amend 修改上一版本的注释并重新提交暂存区


#### checkout + 路径 = 撤销文件操作
git checkout commitHash filename  重置暂存区和工作目录
git checkout -- filename          重置工作目录
