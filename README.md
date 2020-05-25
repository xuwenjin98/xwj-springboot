# xwj-springboot
springboot的学习与记录

git常用命令
git init 初始化
git add xx.txt 或git add * 添加到本地仓库
git commit -m "提交信息"
git remote add git@github.com:lizheng-cn/lizheng-cn.github.io 连接远程仓库
git push-u origin master  / git push


对于一个空目录,创建全新内容
 git init
 //"在此空目录下放入你的文件xx.txt"
 git add xx.txt 或者 git add *
 git commit -m "提交信息"
 git remote add git@github.com:lizheng-cn/lizheng-cn.github.io
 git push-u origin master//如果当前分支与多个主机存在追踪关系，则可以使用-u选项
                         //指定一个默认主机，这样后面就可以不加任何参数使用git push
                         

对于一个空目录,从线上仓库克隆
git clone git@github.com:lizheng-cn/lizheng-cn.github.io //会在当前目录下 
                                                          //生成lizheng-cn.github.io文件夹
 //可进行修改
 git add * //完成所有修改
 git status //查看状态，可省略
 git commit -m "相关信息"
 git push origin master //第一步已经指定了默认主机
 
 
 对于一个已经存在的本地仓库,需要和线上仓库同步
  git pull origin master //fetch and merge 取回线上内容并和本地内容合并
 //开始修改内容
 git add * 
 git commit -m "相关信息"
 git push origin master 