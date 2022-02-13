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