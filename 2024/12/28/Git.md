

#  Git“能用就行”教程

### 1. 下载Git

+ 官网下载放到D盘
+ 将\bin放到用户PATH中
+ 将\usr\bin放到用户PATH中(使得能用Git Bash)

测试节点:

+ git –version
+ 可以配置

### 2. 配置ssh

`git config --global user.name "名字"`
`git config --global user.email "邮箱"`

`ssh-keygen -t rsa -b 4096 -C "邮箱"`
切换到`~/.ssh/rsa.pub`
把`rsa.pub`中的所有东西copy下来

登录`github`找到settings里面的ssh,新开一个key，把刚刚复制的东西放进去

测试节点: 

+ git clone git@xxx.git
+ 常用命令

### 3. 基本常用命令

1. 自定义`git`

`.minttyrc`
`Font=Consolas`
`FontHeight=14`
`Columns=120`
`Rows=40`



`git pull` `github`有更新了，给本地也更新一下

`git add .` 把本地所有东西加到暂存区

`git commit -m "推送信息" `

`git push origin master`第一次这么使用
`git push` 把本地东西推到`github`

Git的逻辑: 工作区，暂存区，版本库
所有修改的文件都在工作区，可以把修改过的文件推到暂存区，可以把暂存区的文件推到版本库

