### 修改操作

#### * 删除文件

* `git rm -f `
  * 将指定的文件，强制从工作目录中删除
* `git rm --cached `
  * 删除 git 已追踪的文件，更改为未追踪的状态

#### * 取消删除

* `git checkout -- `
  * 撤销工作区文件的修改动作
* `git reset HEAD <文件>`
  * 撤销暂存区文件的修改动作
* `git reset --hard HEAD^`
  * **已使用 git commit 提交缓存**情况下，回退到上一次 commit 的状态
* `git reset --hard <commit_id>`
  * 回退到任意版本

#### * 恢复删除内容

* `git reflog`
  * 查看git 历史操作记录
* `git reset `
  * 回退到指定提交的状态，并且工作区的修改 和 已提交的内容修改，会保留
* `git reset --hard 8a0fd74`
  * 回退到指定提交的状态，并且清空工作区和暂存区
