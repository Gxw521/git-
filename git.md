# git常用操作

## start a working area 启动工作区

```md
   clone      Clone a repository into a new directory 克隆到新目录库

   init       Create an empty Git repository or reinitialize an existing one 创建一个空的Git存储库或重新初始化一个现有的存储库

```

## work on the current change处理当前的变化

```md
   add        Add file contents to the index向索引中添加文件内容

   mv         Move or rename a file, a directory, or a symlink移动或重命名文件、目录或链接

   reset      Reset current HEAD to the specified state复位复位电流头到指定状态

   rm         Remove files from the working tree and from the index从工作树和索引中删除文件

```

## examine the history and state检查历史和状态

```md
   bisect     Use binary search to find the commit that introduced a bug使用二进制搜索来查找引入bug的提交

   grep       Print lines matching a pattern匹配图案的GRIP打印行

   log        Show commit logs日志显示提交日志

   show       Show various types of objects显示各种对象

   status     Show the working tree status状态显示工作树状态

```

## grow, mark and tweak your common history成长、标记和调整共同开发历史

```md
 branch     List, create, or delete branches分支列表、创建或删除分支

   checkout   Switch branches or restore working tree files检查交换机分支或恢复工作树文件

   commit     Record changes to the repository向存储库提交记录更改

   diff       Show changes between commits, commit and working tree, etc差异在提交、提交和工作树等之间显示变化

   merge      Join two or more development histories together将两个或多个开发分支记录合并在一起

   rebase     Reapply commits on top of another base tip提交到另一个基础提示的顶部

   tag        Create, list, delete or verify a tag object signed with GPG标记创建、列表、删除或验证用GPG签名的标记对象

```

## collaborate协作

```md
  fetch      Download objects and refs from another repository从另一个存储库获取下载对象和引用

   pull       Fetch from and integrate with another repository or a local branch从另一个存储库或本地分支中提取并集成(下拉)

   push       Update remote refs along with associated objects将更新的远程参考文件连同相关对象一起推送(上传)

```

### 说明

> 'git help -a' and 'git help -g' list available subcommands and some“Git帮助”和“Git帮助-G”列出可用的子命令和一些概念指南
>
> concept guides. See 'git help <command>' or 'git help <concept>'
> to read about a specific subcommand or concept.参见“Git帮助<命令>”或“Git帮助<概念> >
>
> 读取特定的子命令或概念。

## 开发

#### git管理项目

```md
1. git init 本地仓储,生成.git文件夹
2. 远程(github)新建仓储
3. git status 查看仓库状态
4. git add . 全部提交
5. git commit -m "提交名称" 提交到本地
6. git remote add origin 远程仓储地址
7. git push -u origin master origin相当于仓储地址变量，第一次要-u
//完成提交
```

#### 拉出分支工作

```md
> 新建登录分支
	git branch dev-login 新建dev-login分支
> git branch 查看分支
> git checkout dev-login 检出dev-login分支
> 在master分支中合并dev-login分支
	git checkout master 切换到master分支
	git merge dev-login 合并分支
> git branch -d dev-login 删除dev-login分支
!----
> git checkout -b dev-login 创建并检出分支
```

#### 合并分支

```md
> 功能开发完毕，分支是不需要的
	git branch 查看分支
> git checkout master 切换主分支
> git merge dev-login 合并分支
	git branch 查看
> git branch-d dev-login 删除分支
```

