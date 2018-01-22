    1.git checkout -b dev
    2.开发
    3.发布release分支上去
    4.在release上进行测试
    5.直接在release上进行bug修复
    6.修复完成合并到dev、master

    1.再次增减功能时，从dev分支checkout一个feature分支
    2.在feature分支上进行开发，迭代若干版本后，merge到dev分支上，合并时要使用 --no-ff，在dev分支上创建release分支，交测试人员测试
    3.测试出现bug，直接在release上进行修复
    4.回归通过后，release分支同步到dev、master
    5.在master上打tag
    6.这时可以删除featur、releasee分支


标签管理
# 列出所有tag
git tag

# 新建一个tag在当前指定commit
git tag [tag]



