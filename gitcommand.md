## Git learning

### 1. github的访问方式

修改hosts文件 从http://ping.chinaz.com/ft.com 搜索最快速的ip地址

2. ### git命令

   git remote add origin #配置远程git版本库

   ```
   # 增加一个新的远程仓库，并命名
   $ git remote add [shortname] [url]
   ```
   
   git remote -v 显示所有远程仓库地址
   
   git pull origin master #下载代码及快速合并
   
   git push origin master #上传代码及快速合并
   
   git fetch origin		#从远程库获取代码

echo "# gitlearning" >> README.md  echo命令将文本输出  后面指定了输出到一个文件中（readme.md)

git add .  将所有更改放到暂存区

```git
git commit -m "first commit"
```

向本地版本库提交更改

```
git branch -M main
```

将本地分支强制“-M”命名为“main”

git push -u origin main 将本地的main分支提交并覆盖到远程的origin分支（这个origin名称是你在git remote add 时对远程仓库定义的名称）





```shell
$ git push -u origin master


Shell
```

上面命令将本地的`master`分支推送到`origin`主机，同时指定`origin`为默认主机，后面就可以不加任何参数使用`git push`了。

不带任何参数的`git push`，默认只推送当前分支，这叫做`simple`方式。此外，还有一种`matching`方式，会推送所有有对应的远程分支的本地分支。Git 2.0版本之前，默认采用`matching`方法，现在改为默认采用`simple`方式。如果要修改这个设置，可以采用`git config`

```shell
$ git config --global push.default matching
# 或者
$ git config --global push.default simple
```

//原文出自【易百教程】，商业转载请联系作者获得授权，非商业转载请保留原文链接：https://www.yiibai.com/git/git_push.html 

