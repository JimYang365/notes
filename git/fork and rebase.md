# git command

### fork and rebase
https://gist.github.com/ravibhure/a7e0918ff4937c9ea1c456698dcd58aa
在fork的分支上做rebase的方法
1.添加远程分支
git remote add upstream REMOTE
把被fork的原始分支对应到远程分支upstream
2.获取原始分支
git fetch upstream
3.切换到本地主分支
git checkout master
4.从原始分支rebase到当前分支
git rebase upstream/master
5.推送到fork过的远程分支
git push -f origin master
rebase后第一次提交要用push -f，强制提交

