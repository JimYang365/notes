# [在fork的分支上做rebase的方法](https://gist.github.com/ravibhure/a7e0918ff4937c9ea1c456698dcd58aa)

* **通过页面fork到我们自己的仓库**


* **添加远程分支**

```bash
git remote add upstream REMOTE_URL
```

* **获取原始分支**

```bash
git fetch upstream
```

* **切换到本地主分支**

```bash
git checkout master
```

* **从原始分支rebase到当前分支**

```bash
git rebase upstream/master
```

* **推送到fork过的远程分支**

```bash
git push [origin master]
```

* **通过页面生成new merge request**

* **具有merge权限的用户review、merge**


