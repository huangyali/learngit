git is a version control system,is free software,i am stadying.

安装git,命令创建用户邮件地址，生成git仓库地址
在仓库下所有文件都会被git检索到

命令：
cd learngit
git add  file.txt   往仓库添加文件
git commit -m”记录说明”  提交文件
git status 查看当前的状态
git diff 查看修改了什么不同的different内容
git log  查看提交的历史版本号及说明
git reset —-hard HEAD^  返回上一个版本 HEAD^^返回上上一个版本  —-hard 中间不能有空格
cat read.txt  查看文件的内容
git reset —-hard 1a036  返回该版本号 1a036为commit id即版本号
git reflog 查看命令历史，可以记录每一次提交的命令，上面有版本号id
git checkout —- file.txt 撤销到最近的状态（暂存区或版本库） “—-”不能丢掉

如果已经add到暂存区，可以使用这个命令把暂存区的修改退回到工作区
git reset HEAD file.txt 把暂存区退回工作区
git checkout —- file.txt 撤销到最近的一次修改，之前add那一个版本就没有了
