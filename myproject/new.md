## 问题1：

- 1.git push 中remote: Permission to xxxxx.git denied to xxx. fatal: unable to acce

```
由于电脑使用git bash 配过SSH, 系统已经将指向github.com的用户设置之前用户，系统默认读取保存在本地的之前用户
```

- 解决方式：

```
修改.git/config中url:
将
[remote "origin"]
url = https://github.com/git的用户名/项目名称
的url改为
url = https://git的用户名@github.com/git的用户名/项目名称
然后
git push -u origin master
```

## 问题2：

- git切换分支并新建

```
git checkout -b 新分支名字
```

- 只是切换分支

```
git checkout 分支名字
```

## 问题3：

- git配置 .gitignore

```
touch .gitignore
```

- 





## 问题4：

- git忽略logs文件下所有日志文件，但想保留logs文件夹

```
logs文件夹下新建.gitignore，输入如下内容
# ignore all except .gitignore file
*
! .gitignore
```

## 问题5：

- git push报错 fatal: HttpRequestException encountered.▒▒▒▒▒▒▒▒ʱ▒▒▒▒ libpng warning: iCCP: cHRM chunk does not match sRGB Everything up-to-date

  [下载GCMV-1.20.0.exe](https://github.com/microsoft/Git-Credential-Manager-for-Windows/releases)