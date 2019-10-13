```git config --global user.name 'your_name'```
```git config --global user.email 'your_email@domain.com'```



`git remote add <name> <SSH> `        # 添加一个本地与远端的联系



`git add -A`    # 把所有的变化添加进暂存区



```git commit```

`git commit -m 'message'`  

```git commit --amend  ```    # 修改最近一次commit时的message信息



```git rebase -i```   # 修改之前的commit



```git reset --hard ID```       # 清除commit前的操作 也就是清理暂存区 回到这个ID的commit
```git reset HEAD```           # 将暂存区恢复到工作区的内容



```git mv A.py B.py```         # 将A.py文件名修改为B.py



```git help --web log```    # 在网页中查看git log的用法



```git log```
`git log --oneline`     # 按说明查看修改
``git log -n4``        # 查看最近修改的4个操作
`git log master`    # 只查看master分支的操作
`git log --all`     # 查看所有分支的记录
`git log --graph`     # 图形化版本演变



`git branch`     # 创建分支
`git branch -av `     # 查看本地和远端有多少分支
`git branch -D` 分支名     # 删除分支



`git checkout ` # 切换分支
`git checkout -b new_branch master`   # 创建一个名为new_branch的新分支并指向这个分支 这个分支基于master分支 
`git checkout -- <file>`    # 变更工作区内容为暂存区的内容



`git cat-file -p ID`    # 查看ID值对应的内容



`git diff`           # 比较工作区和暂存区的差异
`git diff -- readme.md`          # 比较readme.md中工作区和暂存区的差异
`git diff --cached `    # 比较暂存区和当前HEAD的差异



`git rm <filename>`   # 删除文件



`git stash `           # 临时有任务 可以将工作区的内容先寄存到一个地方  

`git stash apply`       # 将之前在寄存的东西弹出来放在工作区 但是stash列表中还保留这个 pop不保留



`gitk`     # 图形化工具查看版本历史