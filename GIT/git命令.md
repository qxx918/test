**git命令**
1. 克隆项目

   HTTPS：git clone https://github.com/qxx918/smallBillSystem.git

   SSH：git clone git@github.com:qxx918/test.git

2. 初始化git
   git init（主要为了生成 .git 相关文件）

3. 查看git状态（当前分支文件状态）
   git status

4. 查看当前目录下所有文件及文件夹
   ls -ah

5. 拉取代码
   git pull

6. 获取代码/版本库/日志

   git fetch

7. 添加到本地库
   * 提交所有变化
      git add -A （git add --all的缩写）
   * 提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)
      git add -u
   * 提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件
      git add .

8. 提交到远程仓库
   git commit -m "提交描述内容" 
   （注意：git base here有时中文备注不好使，可以使用TortoisteGit客户端、或者使用idea的Terminal终端）

9. 推送到服务器
   git push

   git push -u origin master

10. 删除文件并提交
   git rm 文件名称
   git commit -m "remove 文件名称"   

11. 查看日志
   git log （日志简洁版：git log --pretty=oneline）

12. 将本地文件恢复成远程仓库的文件
   git checkout -- test.txt

   git checkout  finsuit-prd/src/main/java/com/udo/finsuit/service/impl/FinsuitFifawcServiceImpl.java

13. git放弃本地修改、新增、删除的文件

   git checkout . && git clean -df   可以放弃所有修改、删除的文件

   git clean -df   删除新增的文件（未受版本控制的文件）

   -d 表示同时移除目录，-f 表示force强制，因为在git的配置文件中，clean.requireForce=true，如果不加-f，clean将会拒绝执行

14. 如果新增、修改、删除本地文件，那么提交步骤如下：	

   - 先拉取代码

     git pull

   - 添加到本地仓库
     git add -A 

   - 提交到本地服务器
     git commit -m "提交内容"

   - 推送到服务器
     git push

     输入：用户名、密码即可

15. 新建、切换、删除分支

   - 新建分支
      git branch 分支名称（git branch xx），不切换到新分支

      git checkout -b origin/v1.0 ，切换到该分支

   - 查看当前分支

     git branch（带*/绿色字体表示当前分支）

     git branch -a

   - 切换分支

     git checkout 分支名称

   - 删除分支推送到服务器
     

16. 将没有提交的文件放入暂存区

   git stash 把所有没有提交的修改暂存到stash里面。可用git stash pop回复

17. 查看当前分支日志

   git log 

18. 




