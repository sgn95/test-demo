# git rebase 使用

背景： 由于开发一次功能过多的提交，过多的合并，导致git flow 混乱。

提交代码规范，使用git rebase。

使用rebase 优点： 压缩多次提交， 以主分支为基，避免多次merge 导致的git flow 混乱。

如何使用：

step 1:    

    git reabse master -i head~N (N 表示要修改前几次的commit)



step 2:


step 3: