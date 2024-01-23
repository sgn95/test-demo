# git rebase 使用

背景： 由于开发一次功能过多的提交，过多的合并，导致git flow 混乱。

提交代码规范，使用git rebase。

使用rebase 优点： 压缩多次提交， 以主分支为基，避免多次merge 导致的git flow 混乱。

如何使用：

step 1:    

    git reabse -i head~N (N 表示要修改前几次的commit)


step 2:

    git rebase dev 

step 3:

    遇到冲突 需要解决冲突  git add ‘’

step 4:

    git rebase --continue
    
注意： 修改内容需要按照标准的格式：
``` 
    feat: 增加新功能
    fix: 修复bug
    modify: 修改一些需求
    docs: 对文档的修改
    style: 代码格式上的变动
    refactor: 重构 不新增 也不修改bug
    perf：优化相关 
    test: 增加测试
    revert： 回滚版本
```