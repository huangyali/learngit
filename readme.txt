git is a version control system,is free software,i am stadying.
分布式版本系统的是在本地工作完全不需要考虑远程库的存在，也就是有没有联网都可以正常工作，
而SVN在没有联网的时候是拒绝干活的！当有网络的时候，再把本地提交推送一下就完成了同步，真是太方便了！
git教程：http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000

安装git,命令创建用户邮件地址，生成git仓库地址
在仓库下所有文件都会被git检索到

命令：
cd learngit
git add  file.txt        往仓库添加文件
git commit -m”记录说明”    提交文件
git status               查看当前的状态
git diff                 查看修改了什么不同的different内容
git log                  查看提交的历史版本号及说明
git reset —-hard HEAD^   返回上一个版本 HEAD^^返回上上一个版本  —-hard 中间不能有空格
cat read.txt             查看文件的内容
git reset —-hard 1a036   返回该版本号 1a036为commit id即版本号
git reflog               查看命令历史，可以记录每一次提交的命令，上面有版本号id
git checkout —- file.txt 撤销到最近的状态（暂存区或版本库） “—-”不能丢掉

如果已经add到暂存区，可以使用这个命令把暂存区的修改退回到工作区
git reset HEAD file.txt  把暂存区退回工作区
git checkout —- file.txt 撤销到最近的一次修改，之前add那一个版本就没有了

删除文件
git rm file.txt 删除文件， git commit提交后版本库也会删除
如果版本库中还有这个文件，通过git checkout —- file.txt 可以从版本库中恢复到工作区

使用GitHub仓库，在官网上添加一个ssh key,往仓库推送东西，需要这个key，不同的电脑使用一个github仓库可以分别在电脑上注册key 
创建key命令，ssh-keygen -t rsa -C “youremail@example.com”

切入本地learngit仓库，把本地仓库与远程github中的origin仓库相连接
git remote add origin https://github.com/huangyali/learngit.git
git push origin master

从现在起，只要本地作了提交，就可以通过命令：
$ git push origin master一次推送master分支的所有内容

从github仓库中克隆到本地一个仓库
先切入自己本地learngit仓库
$ git clone git@github.com:huangyali/learngit.git
这样本地就会把github上learngit仓库下所有内容克隆在本地

git创建修改文件，无论文件是一个还是一万个，速度非常快，一秒钟完成，比其他版本控制系统快

git创建另一个分支dev，在dev上做修改，再把dev上修改的内容提交到master上
git branch           查看所有分支，带*号的为当前分支
git branch name      创建分支 name为分支名字
git checkout name    切换分支
git checkout -b name 创建并切换分支
git merge name       合并某（name）分支到当前分支，因为先切换到你要合并到的分支上
git branch -d name   删除分支
git branch -D name   强制删除分支

git stash            保存当前工作内容 （不用提交，切换到其他分支，该内容不会丢失）
git stash apply      恢复刚才stash保存的内容,不会删除
git stash pop        恢复并删除stash内容

git config —-global user.name “huangyali”
git config —-global user.email “yalihuang214@163.com”
git remote     查看远程库的信息
git remote -v  显示远程库抓取和推送的origin地址

多人都在远程库上克隆主分支 master，开发在新建分支dev上
如果两人都分别在dev分支上修改同一个文件，一个人push成功，另一个人就得先抓取pull下来，再push推送
git pull 从远程库上抓取该文件内容，就是svn的更新
git branch —-set-upstream dev origin/dev  pull有可能失败，要设置本地dev分支和远程origin/dev分支的链接，再git pull,pull成功，合并有冲突，手动解决，再push上去

git tag name 新建一个标签
git tag -a tagname -m “标签信息”
git tag     查看所有标签
