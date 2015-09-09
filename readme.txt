git is a version control system,is free software,i am stadying.
安装git,命令创建用户邮件地址，生成git仓库地址
在仓库下所有文件都会被git检索到
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