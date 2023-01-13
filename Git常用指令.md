# 常用指令

**新建仓库：**

* git init
* ssh-keygen -t rsa(不断回车)
* cat ~/.ssh/id_rsa.pub（获取公钥）
* 配置SSH公钥
* ssh -T git@gitee.com（验证公钥是否成功）
* git remote add origin git@gitee.com:（）

重要指令:工作流程git remote add origin git@gitee.com:czbk_zhang_meng/git_test.git图上的7个指令(clone+fetch+pull+checkout+add+push+commit)

命令如下：

1. clone（克隆）: 从远程仓库中克隆代码到本地仓库

2. checkout （检出）:从本地仓库中检出一个仓库分支然后进行修订

3. add（添加）: 在提交前先将代码提交到暂存区

4. commit（提交）: 提交到本地仓库。本地仓库中保存修改的各个历史版本

5. fetch (抓取) ： 从远程库，抓取到本地仓库，不进行任何的合并动作，一般操作比较少。
6. pull (拉取) ： 从远程库拉到本地库，自动进行合并(merge)，然后放到到工作区，相当于fetch+merge

7. push（推送） : 修改完成后，需要和团队成员共享代码时，将代码推送到远程仓库

常用指令速查:

​	-基本操作类:
​						git init	初始化仓库
​						git-log	**查看日志，这个命令很重要!!!!!!!!!!!**
​						git add <文件名>	添加到暂存区
​						git commit -m '注释‘	提交到仓库	
​						git merge<分支名>	合并指定分支到当前活跃分支
​	-分支切换类：
​						git checkout<分支名>	切换到某个分支
​						git checkout -b<分支名>	创建并切换到某个分支（分支原来不存在）

​	-远程操作：
​						git clone <远程地址> [本地文件夹]	clone远程仓库到本地
​						git pull	拉取远端仓库的修改并合并
​						**git push [--set-upstream] origin 分支名	推送本地修改到远端分支**
**​										-set-upstream表示推送到远端的同时并且建立起和远端分支的关联关系。**

​	-版本回退：

​						git reset --hard commitID	

​														版本切换（commitID 可以使用 git-log 或 git log 指令查看）

​						git reflog 查看已经删除的记录