### 标签操作

#### * 创建标签

* git tag `<tag-name>`

  * 在当前分支的最新commit上，添加标签
  * 标签名：v `<major>`.`<minor>`.`<patch>`
    * major（主版本号）：重大变化
    * minor（次要版本号）：版本与先前版本兼容
    * patch（补丁号）：bug修复
* git tag `<tag-name>` `<commit-id>`

  * 给指定commit 创建标签
* git tag -a `<tagname>` -m "`<message>`"

  * 给标签名 添加备注信息
  * -a, --annotate        附注标签，需要一个说明
  * -m, --message <说明>  标签说明

#### * 查看标签信息

* git tag -n
  * -n[`<n>`]  每个标签信息打印 `<n>` 行

#### * 切换到指定标签的commit

* git reset --hard `<tag-name>`

#### * 删除标签

* git tag -d `<tag-name>`
* git push origin -d `<tag-name>`
  * 删除远程仓库的指定标签：

#### * 拉取标签

* git fetch --tags
  * 将远程仓库的标签拉取（同步）到当前分

#### * 从指定标签所在commit，切出分支

* git checkout -b `<branch> <tag-name>`
