---
layout: post
title:  "Welcome2"
date:   2017-03-02 17:05:13 +0000
categories: jekyll update
---


Git �ֲ�ʽ�汾����ϵͳ

���ؿ�  +  githubԶ�̿�

���ؿ⣺
��������δ���棩 + �м��������棩+ �����������棩


Github
������Զ�� ���⣺

*     ����Զ������----��¡----�Լ�Զ������-----get---��������

*     ����Զ������----��¡----�Լ�Զ������
��Fork�������Լ����˺��¿�¡��һ��bootstrap�ֿ�



git���ԭ��

ͨ�� �� �м����� �� ��������ֿ⡱ ���а汾����
�޸ĵ��ļ����������add���м���stage�� Ȼ�����ύcommit�����ֿ�

���Խ����޸ģ����ˣ�ɾ�����ύ�Ȱ汾����


��������δ�ύ���ļ�

�ݴ������м仺���ļ���add�ύ���

Master��ʽ���� ��ʽ�ύ�����ļ���commit�ύ��

ΪʲôGit����ļ���Ҫadd��commitһ�������أ�
��Ϊcommit����һ���ύ�ܶ��ļ�����������Զ��add��ͬ���ļ�




ʹ�ã�

#ע��
 ȫ���û�����ȫ���ʼ���ϵ��

$ git config --global user.name "Your Name"$ git config --global user.email "email@example.com"


#�����¿�, ��Ϊ��repository
(���ǹ���Ŀ¼���ļ��İ汾)
init
��ʼ����
ѡ��һ��Ŀ¼��Ϊ�¿�
ʹ��git init
$ git init





Add
�����ļ�����Ŀ¼
Ȼ��ע����ӵ�git���м���
$ git add readme.txt


Commit
ʹ��commit�İ������м����ļ��ύ������
$ git commit
$ git commit -m "wrote a readme file"


Checkout
���ǻ��ˣ�����ȡ��������ǰ���µ�һ���汾
1�����˺�����һ��
2�������ǻ��˺� �м��� һ�£����������ύ���м���


��ǩtag
��������ĳ��ʱ�̵İ汾��
��commit�������ǣ���ǩ�����ƣ�commit�����ֲ����׼���

��֦
����һ������汾







Github
������Զ�� ���⣻

����Զ������----��¡----�Լ�Զ������-----get---��������

git��ʹ�����ַ������̣�
��1������ĳ������Ŀ¼�£�Ȼ�󴴽��¿⣩
��2����Զ��github�����¿⣬Ȼ���ٴ�������Ŀ¼�����ͬ�������أ�

һ��ʹ�ò��裬Զ��github�����տ⣬Ȼ���¡�ر���
��Ҳ���Ա����ȴ�����Ŀ¼��Ȼ��Զ�̴����⣬Ȼ�����������


ȫ��ʹ�ã�

��װgit ->  ע�᱾���û� ->����SSH��Կ->ע��Զ��github->Զ��github�Ǽ�SSH��Կ
->��¡Զ�̿�ر���->�޸��ļ�->�ύͬ��

#��װgit

#ע��
 ȫ���û�����ȫ���ʼ���ϵ��

$ git config --global user.name "Your Name"$ git config --global user.email "email@example.com"



#github��Զ������
Git�����ʺ�ͨ��SSH���ӵ� SSH Key����¼����
���ر���id_rsa ����Կ  �� Զ�̵Ǽ�id_rsa.pub �ǹ�Կ����Ե�¼����


#������Կ
$ssh-keygen -t rsa 

��˼��ָ�� rsa �㷨������Կ���������������س���������Ҫ�������룩��
�����������ļ� id_rsa �� id_rsa.pub ��
id_rsa ����Կ��id_rsa.pub �ǹ�Կ��
�������ļ�Ĭ�Ϸֱ�������Ŀ¼�����ɣ�
Linux/Mac ϵͳ �� ~/.ssh �£�
��Կ���ر���Ŀ¼��
winϵͳ�� /c/Documents and Settings/username/.ssh
/c/Users/shawnzhuo/.ssh/

#Զ��github�Ǽ�
 ��github�ϵǼ�id_rsa.pub �ǹ�Կ�ĵ�ַ
GitHub -������-����� SSH and GPG keys ��

�� Key ������ id_rsa.pub ��Կ�ļ�������ݸ���ճ����ȥ


#Ҫ����һ��Զ�̿⣬ʹ������
git remote add origin git@server-name:path/repo-name.git��
git remote add origin git@github.com:shawnzhuo/learngit.git
Զ�̿�����־���origin������GitĬ�ϵĽз�


#������ʹ�������һ������master��֧���������ݣ�
git push -u origin master
��ǰ��֧master���͵�Զ�̡�-u������Git������ѱ����������͵�Զ�̣������Զ��������


#�˺�ÿ�α����ύ��ֻҪ�б�Ҫ���Ϳ���ʹ���������������޸ģ�
git push origin master


#github��¡�����ؿ�
git clone git@github.com:shawnzhuo/gitskills.git











GitHub ��һ�㶼�ǻ��� SSH ��Ȩ�ġ�
��ôʲô�� SSH �أ�

�򵥵�˵��SSH��һ������Э�飬���ڼ����֮��ļ��ܵ�¼��Ŀǰ��ÿһ̨ Linux ���Եı�׼���á�������� Git ����������ѡ��ʹ�� SSH ��Կ��������Ȩ��������Ҫ�� GitHub �ύ����ĵ�һ������Ҫ����� SSH key ����

������Կ
$ssh-keygen -t rsa 
��˼��ָ�� rsa �㷨������Կ���������������س���������Ҫ�������룩��
�����������ļ� id_rsa �� id_rsa.pub ��
id_rsa ����Կ��id_rsa.pub �ǹ�Կ��
�������ļ�Ĭ�Ϸֱ�������Ŀ¼�����ɣ�
Linux/Mac ϵͳ �� ~/.ssh �£�winϵͳ�� /c/Documents and Settings/username/.ssh


������Ҫ�����ǰ� id_rsa.pub ��������ӵ� GitHub �ϣ��������ص� id_rsa ��Կ�� GitHub �ϵ� id_rsa.pub ��Կ������ԣ���Ȩ�ɹ��ſ����ύ���롣


GitHub�����SSH Key
������ GitHub �ϵ�����ҳ�棬�������� SSH and GPG keys ��
Ȼ�������Ͻǵ� New SSH key ��ť��


��Ҫ����ֻ���� Key ������ id_rsa.pub ��Կ�ļ�������ݸ���ճ����ȥ�Ϳ����ˣ�����ʾ��Ϊ�˰�ȫճ���Ĺ�Կ����Ч�ģ���Title ������Ҫ��д����� Add SSH key ��ť��ok�ˡ�










