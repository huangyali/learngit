git is a version control system,is free software,i am stadying.
�ֲ�ʽ�汾ϵͳ�����ڱ��ع�����ȫ����Ҫ����Զ�̿�Ĵ��ڣ�Ҳ������û����������������������
��SVN��û��������ʱ���Ǿܾ��ɻ�ģ����������ʱ���ٰѱ����ύ����һ�¾������ͬ��������̫�����ˣ�


��װgit,������û��ʼ���ַ������git�ֿ��ַ
�ڲֿ��������ļ����ᱻgit������

���
cd learngit
git add  file.txt   ���ֿ�����ļ�
git commit -m����¼˵����  �ύ�ļ�
git status �鿴��ǰ��״̬
git diff �鿴�޸���ʲô��ͬ��different����
git log  �鿴�ύ����ʷ�汾�ż�˵��
git reset ��-hard HEAD^  ������һ���汾 HEAD^^��������һ���汾  ��-hard �м䲻���пո�
cat read.txt  �鿴�ļ�������
git reset ��-hard 1a036  ���ظð汾�� 1a036Ϊcommit id���汾��
git reflog �鿴������ʷ�����Լ�¼ÿһ���ύ����������а汾��id
git checkout ��- file.txt �����������״̬���ݴ�����汾�⣩ ����-�����ܶ���

����Ѿ�add���ݴ���������ʹ�����������ݴ������޸��˻ص�������
git reset HEAD file.txt ���ݴ����˻ع�����
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

