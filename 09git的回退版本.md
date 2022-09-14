### git的回退版本

git reset -soft HEAD~     版本回到上一次提交版本，其他内容都不变
  git reset -soft xxx     版本回到指定版本，其他内容都不变
git reset --mixed HEAD~   版本回到上一次提交版本，同时改变暂存区内容，工作区不变
  git reset --mixed xxx   ... ...
git reset --hard HEAD~    版本回到上一次提交版本，同时改变暂存区和工作区内容
  git reset --hard xxx   ... ...
  对于有未暂存的文件，直接操作--hard会导致文件永久丢失，慎用！
  git branch recover-branch xxx 恢复指定版本并创建新分支,recover-branch是新分支名

