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