# 配置公私钥
localhost:
    ssh-keygen -t rsa -C '1084176474@qq.com'

# github添加配置公钥

# 同步github，github中含有文件
git fetch github master
git merge --allow -unrelated-histories github master
git push github master

