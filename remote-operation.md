### 远程操作

#### * 本地初始化的git仓库，添加或移除远程仓库的关联关系

* `git remote add <remote_name> <remote_url>`
  * `remote_name`：仓库名称（默认是origin）
  * `remote_url：远程仓库地址`（如：git@github.com:jellyzhai/git-practice.git）
* `git remote rm origin`
  * 从本地移除远程仓库的记录（也就是解除本地仓库和远程仓库的关系），并不会真正影响到远程仓库。

#### * 查看远程仓库

* `git remote -v`

#### * 从远程仓库拉取分支代码

* 将**与本地当前分支同名的远程分支**拉取到**本地当前分支上：**
  * `git pull`
* **远程指定分支**拉取到 **本地当前分支上** ：
  * `git pull origin <远程分支名>`
* 将**远程指定分支**拉取到 **本地指定分支上** (没有的本地分支，会新建)：
  * `git pull origin <远程分支名>:<本地分支名>`

#### * 本地提交的commit，推送到远程仓库分支

* 来将本地分支与远程同名分支相关联：
  * `git push -u origin <本地分支名>`
    * -u = --set-upstream 设置上游
* 将**本地当前分支**推送到 **与本地当前分支同名的远程分支上** ：
  * `git push`
* 将**本地指定分支**推送到 **远程指定分支上** ：
  * `git push origin <本地分支名>:<远程分支名>`
