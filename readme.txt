git is a version control system,is free software,i am stadying.
�ֲ�ʽ�汾ϵͳ�����ڱ��ع�����ȫ����Ҫ����Զ�̿�Ĵ��ڣ�Ҳ������û����������������������
��SVN��û��������ʱ���Ǿܾ��ɻ�ģ����������ʱ���ٰѱ����ύ����һ�¾������ͬ��������̫�����ˣ�
git�̳̣�http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000

��װgit,������û��ʼ���ַ������git�ֿ��ַ
�ڲֿ��������ļ����ᱻgit������

���
cd learngit
git add  file.txt        ���ֿ�����ļ�
git commit -m����¼˵����    �ύ�ļ�
git status               �鿴��ǰ��״̬
git diff                 �鿴�޸���ʲô��ͬ��different����
git log                  �鿴�ύ����ʷ�汾�ż�˵��
git reset ��-hard HEAD^   ������һ���汾 HEAD^^��������һ���汾  ��-hard �м䲻���пո�
cat read.txt             �鿴�ļ�������
git reset ��-hard 1a036   ���ظð汾�� 1a036Ϊcommit id���汾��
git reflog               �鿴������ʷ�����Լ�¼ÿһ���ύ����������а汾��id
git checkout ��- file.txt �����������״̬���ݴ�����汾�⣩ ����-�����ܶ���

����Ѿ�add���ݴ���������ʹ�����������ݴ������޸��˻ص�������
git reset HEAD file.txt  ���ݴ����˻ع�����
git checkout ��- file.txt �����������һ���޸ģ�֮ǰadd��һ���汾��û����

ɾ���ļ�
git rm file.txt ɾ���ļ��� git commit�ύ��汾��Ҳ��ɾ��
����汾���л�������ļ���ͨ��git checkout ��- file.txt ���ԴӰ汾���лָ���������

ʹ��GitHub�ֿ⣬�ڹ��������һ��ssh key,���ֿ����Ͷ�������Ҫ���key����ͬ�ĵ���ʹ��һ��github�ֿ���Էֱ��ڵ�����ע��key 
����key���ssh-keygen -t rsa -C ��youremail@example.com��

���뱾��learngit�ֿ⣬�ѱ��زֿ���Զ��github�е�origin�ֿ�������
git remote add origin https://github.com/huangyali/learngit.git
git push origin master

��������ֻҪ���������ύ���Ϳ���ͨ�����
$ git push origin masterһ������master��֧����������

��github�ֿ��п�¡������һ���ֿ�
�������Լ�����learngit�ֿ�
$ git clone git@github.com:huangyali/learngit.git
�������ؾͻ��github��learngit�ֿ����������ݿ�¡�ڱ���

git�����޸��ļ��������ļ���һ������һ������ٶȷǳ��죬һ������ɣ��������汾����ϵͳ��

git������һ����֧dev����dev�����޸ģ��ٰ�dev���޸ĵ������ύ��master��
git branch           �鿴���з�֧����*�ŵ�Ϊ��ǰ��֧
git branch name      ������֧ nameΪ��֧����
git checkout name    �л���֧
git checkout -b name �������л���֧
git merge name       �ϲ�ĳ��name����֧����ǰ��֧����Ϊ���л�����Ҫ�ϲ����ķ�֧��
git branch -d name   ɾ����֧
git branch -D name   ǿ��ɾ����֧

git stash            ���浱ǰ�������� �������ύ���л���������֧�������ݲ��ᶪʧ��
git stash apply      �ָ��ղ�stash���������,����ɾ��
git stash pop        �ָ���ɾ��stash����

git config ��-global user.name ��huangyali��
git config ��-global user.email ��yalihuang214@163.com��
git remote     �鿴Զ�̿����Ϣ
git remote -v  ��ʾԶ�̿�ץȡ�����͵�origin��ַ

���˶���Զ�̿��Ͽ�¡����֧ master���������½���֧dev��
������˶��ֱ���dev��֧���޸�ͬһ���ļ���һ����push�ɹ�����һ���˾͵���ץȡpull��������push����
git pull ��Զ�̿���ץȡ���ļ����ݣ�����svn�ĸ���
git branch ��-set-upstream dev origin/dev  pull�п���ʧ�ܣ�Ҫ���ñ���dev��֧��Զ��origin/dev��֧�����ӣ���git pull,pull�ɹ����ϲ��г�ͻ���ֶ��������push��ȥ

git tag name �½�һ����ǩ
git tag -a tagname -m ����ǩ��Ϣ��
git tag     �鿴���б�ǩ
