git init               初始化新仓库
git add ./             将文件添加到暂存区
git commit -m "xxx"    提交暂存区文件到版本库
git commit -a -m "xxx" 跳过暂存区
git rm xxx             删除文件（直接修改到暂存区）
git mv xxx xxx         文件改名（直接修改到暂存区）
git log                查看日志 q键退出
  git log --pretty=oneline
  git log --oneline
git reflog             查看完整日志
