```shell
##本地初始化仓库
git init
##本地编辑完文本内容后，提交到暂存区
git add edit.txt / git add . (将当前路径下的所有内容都提交)
##查看当前工作区状态
git status
##绿色代表有文件已提交至暂存区/红色代表有文件没有提交至暂存区

##从暂存区中删除某文件
##比如：不小心把没用的文件提交到暂存区了，想删除时
git rm --cached edit.txt

##强制将本地工作区和暂存区删除某文件
git rm -f edit.txt

##将暂存区中指定内容提交至本地仓库/将暂存区所有内容提交至本地仓库
git commit -m 'add all diff txt' 
git commit edit.txt -m 'add edit.txt to local repository'

##将暂存区的内容提交至本地库时，需要指定用户名和email
##当不指定--global时，则仅对当前仓库有效
git config --global user.name 'runoob'
git config --global user.email test@runoob.com

##查看提交到本地仓库的head指针
git log

##需要本地仓库进行版本回退
git reset xxxxx(版本号)

##需要将本地仓库的内容覆盖回工作区，则指定--hard
git reset --hard xxxxx(版本号)

##将本地仓库内容覆盖工作区，所有的则使用*
git checkout -- (filename)

##当回退到旧版本后，找不到新版本的id时，则使用以下命令
git reflog

##


```

