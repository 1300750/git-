### git分支
git branch        显示分支列表
git branch xxx    创建分支
git checkout xxx  切换分支
git branch -d xxx 删除分支
  git branch -D xxx 强制删除分支
git branch xxx commitHash 新建分支并使分支指向指定提交版本
git log --oneline --decorate --graph --all 查看项目分支历史情况
  git config --global alias.xxx "log --oneline --decorate --graph --all" 配别名
git checkout -b xxx 新建分支并且切换分支

### 切换分支
切换分支会改变工作区和暂存区
每次切换分支前一定是在提交版本后，即git status要保证clean，否则会污染分支

### 合并分支
git merge xxx
  有可能会出现代码冲突，根据提示位置修改完冲突后再git add ./ 再 git commit -m "xxx"

### 分支存储
git stash list 查看存储
git stash 提交存储
git stash pop 应用存储并且立即删除它
  git stash apply 应用存储
  git stash drop stash@{0}删除存储
