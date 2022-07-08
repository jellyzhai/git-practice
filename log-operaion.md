### log日志操作

#### * 按作者查看

* git log --author='username'
  * 查看某个作者的提交
* git log --author='username1 \\| username2'
  * 查看多个作者的提交
* git log --author='username1 \\| username2' --oneline
  * 每个作者信息，按一行概要信息展示

#### * 按时间查看

* git log --after=`<date>`
  * 某个日期之后
* git log --before=`<date>`
  * 某个日期之前
* git log --after='2022.06.01' --before='2022.06.07' --oneline
  * 开始和结束日期直接的日志，按一行显示概要信息

#### * 按文件查看

* git log -- `<path>`
  * 查看某个文件都在哪些提交中修改了内容

#### * 按合并查看

* git log --merges
  * 只查看代码合并的记录
* git log --no-merges
  * 查看非合并操作的操作记录

#### * 按分支查看

* git log master..test
  * 查看 test 分支，比 master 分支，多了哪些提交
* git log master..test
  * 查看 master 分支，比 test 分支，多了哪些提交

#### * 美化日志

* git log --graph --oneline --decorate

#### * 其他参数标志

* git log --oneline
  * 简化日志 一行输出
* git log --stat
  * 简要显示文件增改行数统计
* git log -N
  * `-N`标志来仅显示最近N次的提交
* git log -p
  * 显示每次提交的内容差异对比
