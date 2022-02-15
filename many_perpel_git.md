# 不同的人修改了不同文件处理
git fetch github
git merge github/master
git push github master

# 不同的人修改了同一文件的不同区域
git fetch github
git merge github/master
git push github master

# 不同的人修改了同一文件的同一区域
git pull
git merge github/dev
# 需要手动修改文件选择保留内容后commit
git push github master

# 同时变更文件名和文件内容处理

# 把同一文件改成不同文件名处理