# git全局配置
git config --global user.name 'username'
git config --global user.email 'email'

# git 仓库配置
git init

# 多个文件提交暂存区
git add .
# 单个文件夹/文件提交暂存区
git add filename

# 提交仓库
git commit -m 'first commit'
# 直接提交
git commit -am 'commit'

# 文件重命名
git mv src_filename des_filename

# 查看版本演变历史
git log
# 只查看提交注释
git log --oneline
# 查看最近几次提交
git log -n2
# 查看所有分支图形化日志
git log --all --graph

# 

