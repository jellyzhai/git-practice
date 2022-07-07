### 分支

#### * 本地仓库创建的分支，更新到远程仓库

* git push -u origin `<本地创建的branch>`

  * -u = --set-upstream

#### * 查看贡献者提交代码次数

* git shortlog -sn --no-merge

  * s：省略每次 commit 的注释，仅仅返回一个简单的统计。
  * n：按照 commit 数量从多到少的顺利对用户进行排序。
  *
