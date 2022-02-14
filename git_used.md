# 删除不需要的分支
git branch -d branch_name

# 修改最新commit的message
git commit --amend

# 修改老旧commit的message
git rebase -i 需修改的commit上一次commit哈希值

# 合并连续的commit
git rebase -i 需修改合并的最先的commit的上一次commit哈希值

# 合并不连续的commit
git rebase -i 需修改合并的最先的commit的上一次commit哈希值，然后移动pick行

# 比较暂存区和HEAD所含文件的差异
git diff --cached

# 比较暂存区和工作区文件的差异
git diff

# 如何让暂存区恢复成HEAD一样
git reset HEAD

# 如何让工作区恢复成和暂存区一样
git checkout -- file

# 取消暂存区部分文件的更改
git reset HEAD -- file
git restore --staged file

# 消除最近的几次提交
git reset --hard commit_hash

# 比较commit之间的差异
git diff commit_hash commit_hash -- .

# 正确删除文件
git rm -rf file

# 将工作区暂时恢复成暂存区
git stash

# 恢复暂时存放文件
git stash apply
git stash pop

# 指定不需要git管理的文件，gitignore里的内容与文件名相同时文件不会被git管控
vim .gitignore

# 备份git仓库到本地
git clone --bare file:///git_repo.git backup.git

# 同步远端仓库
git remote add/rm origin  git@github.com:wjamx/MyProject.git
git push origin