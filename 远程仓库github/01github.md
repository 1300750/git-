<!-- 项目经理做的 -->
git remote add xxx url 配置远程仓库并别名
... ... 
git push [romote-name] [branch-name] 推送本地项目到远程仓库
  推送时自动生成远程跟踪分支（新分支名，与master分支并列）
git fetch xxx 更新内容
  会下载远程跟踪分支，但没有本地分支，因此没有对应的本地文件
  所以要创建一个本地分支并合并远程跟踪分支才能真正获取到文件
git branch -vv 查看本地跟踪远程分支列表
git pull xxx 直接拉取文件
  前提是本地分支要跟踪远程跟踪分支：git branch -u xxx(远程分支名)
​	  或 git checkout --track origin/xxx 直接创建本地分支并拉取文件

<!-- 普通员工要做的 -->
git clone url   克隆（自动跟踪master）
git branch -vv 查看本地跟踪远程分支列表
git pull xxx 直接拉取文件
  前提是本地分支要跟踪远程跟踪分支：git branch -u xxx(远程分支名)
​	  或 git checkout --track origin/xxx 直接创建本地分支并拉取文件
git push origin 推送
  推送时自动生成远程跟踪分支（新分支名，与master分支并列）

<!-- 其他操作 -->
git branch:查看本地所有分支
git branch -a:查看本地和远程仓库的所有分支
git branch -r:查看所有远程分支
git push origin --delete serverfix 删除远程分支
git remote prune origin --dry-run 列出仍在远程跟踪但远程已被删除的分支
git remote prune origin 清除上面命令列出来的远程跟踪

