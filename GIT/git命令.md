**git命令**
1. 克隆项目
   git clone https://github.com/qxx918/smallBillSystem.git

2. 初始化git
   git init

3. 查看git状态（当前分支，文件状态）
   git status

4. 查看当前目录下所有文件及文件夹
   ls -ah

5. 拉取代码
   git pull

6. 添加到本地库
   * 提交所有变化
      git add -A （git add --all的缩写）
   * 提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)
      git add -u
   * 提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件
      git add .

7. 提交到远程仓库
   git commit -m "提交描述内容" 
   （git base here有时候中文备注不好使，可以使用TortoisteGit客户端、或者使用idea的Terminal）

8. 推送到服务器
   git push

   git push -u origin master

9. 删除文件并提交
   git rm 文件名称
   git commit -m "remove 文件名称"   （注意：git base here 创建输入中文，会有问题，但使用idea中的终端terminal可以是中文）

10. 查看日志
  git log （日志简洁版：git log --pretty=oneline）

11. 将本地文件恢复成远程仓库的文件
   git checkout -- test.txt

   git checkout  finsuit-prd/src/main/java/com/udo/finsuit/service/impl/FinsuitFifawcServiceImpl.java

12. git放弃本地修改、新增、删除的文件

   git checkout . && git clean -df   可以放弃所有修改、删除的文件

   git clean -df   删除新增的文件（未受版本控制的文件）

   -d 表示同时移除目录，-f 表示force强制，因为在git的配置文件中，clean.requireForce=true，如果不加-f，clean将会拒绝执行。

13. abc




