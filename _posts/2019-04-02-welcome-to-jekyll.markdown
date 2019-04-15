---
layout: post
title:  "Welcome  shawnzhuo"
date:   2017-03-02 17:05:13 +0000
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Git 分布式版本管理系统

本地库  +  github远程库

本地库：
工作区（未保存） + 中间区（缓存）+ 主库区（保存）


Github
互联网远程 主库：

*     别人远程主库----克隆----自己远程主库-----get---本地主库

*     别人远程主库----克隆----自己远程主库
“Fork”就在自己的账号下克隆了一个bootstrap仓库



git理解原理

通过 “ 中间区” 和 “主保存仓库” 进行版本管理，
修改的文件，需先添加add到中间区stage， 然后再提交commit到主仓库

可以进行修改，回退，删除，提交等版本管理


工作区，未提交的文件

暂存区，中间缓存文件，add提交后的

Master正式区， 正式提交保存文件，commit提交后

为什么Git添加文件需要add，commit一共两步呢？
因为commit可以一次提交很多文件，所以你可以多次add不同的文件




使用：

#注册
 全局用户名，全局邮件联系人

$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"


#创建新库, 因为叫repository
(就是管理目录和文件的版本)
init
初始化：
选择一个目录作为新库
使用git init
$ git init





Add
拷贝文件到库目录
然后注册添加到git的中间区
$ git add readme.txt


Commit
使用commit的把所有中间区文件提交到主库
$ git commit
$ git commit -m "wrote a readme file"


Checkout
就是回退（或者取出）到当前最新的一个版本
1、回退和主库一致
2、另外是回退和 中间区 一致，条件是已提交到中间区


标签tag
就是主库某个时刻的版本号
与commit的区别是，标签是名称，commit是数字不容易记忆

分枝
另起一个主库版本







Github
互联网远程 主库；

别人远程主库----克隆----自己远程主库-----get---本地主库

git的使用两种方法流程：
（1、进入某个本地目录下，然后创建新库）
（2、在远程github创建新库，然后再创建本地目录，最后同步到本地）

一般使用步骤，远程github创建空库，然后克隆回本地
（也可以本地先创建库目录，然后远程创建库，然后关联起来）


全新使用：

安装git ->  注册本地用户 ->生成SSH密钥->注册远程github->远程github登记SSH公钥
->克隆远程库回本地->修改文件->提交同步

#安装git

#注册
 全局用户名，全局邮件联系人

$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"



#github的远程连接
Git密码帐号通过SSH连接的 SSH Key来登录访问
本地保存id_rsa 是密钥  和 远程登记id_rsa.pub 是公钥来配对登录访问


#生成密钥
$ssh-keygen -t rsa 

意思是指定 rsa 算法生成密钥，接着连续三个回车键（不需要输入密码）就
会生成两个文件 id_rsa 和 id_rsa.pub ，
id_rsa 是密钥，id_rsa.pub 是公钥。
这两个文件默认分别在如下目录里生成：
Linux/Mac 系统 在 ~/.ssh 下，
密钥本地保存目录：
win系统在 /c/Documents and Settings/username/.ssh
/c/Users/shawnzhuo/.ssh/

#远程github登记
 到github上登记id_rsa.pub 是公钥的地址
GitHub -》设置-》左侧 SSH and GPG keys ：

在 Key 那栏把 id_rsa.pub 公钥文件里的内容复制粘贴进去


#要关联一个远程库，使用命令
git remote add origin git@server-name:path/repo-name.git；
git remote add origin git@github.com:shawnzhuo/learngit.git
远程库的名字就是origin，这是Git默认的叫法


#关联后，使用命令第一次推送master分支的所有内容；
git push -u origin master
当前分支master推送到远程。-u参数，Git不但会把本地内容推送的远程，还会和远关联起来


#此后，每次本地提交后，只要有必要，就可以使用命令推送最新修改；
git push origin master


#github克隆到本地库
git clone git@github.com:shawnzhuo/gitskills.git











GitHub 上一般都是基于 SSH 授权的。
那么什么是 SSH 呢？

简单点说，SSH是一种网络协议，用于计算机之间的加密登录。目前是每一台 Linux 电脑的标准配置。而大多数 Git 服务器都会选择使用 SSH 公钥来进行授权，所以想要在 GitHub 提交代码的第一步就是要先添加 SSH key 配置

生成密钥
$ssh-keygen -t rsa 
意思是指定 rsa 算法生成密钥，接着连续三个回车键（不需要输入密码）就
会生成两个文件 id_rsa 和 id_rsa.pub ，
id_rsa 是密钥，id_rsa.pub 是公钥。
这两个文件默认分别在如下目录里生成：
Linux/Mac 系统 在 ~/.ssh 下，win系统在 /c/Documents and Settings/username/.ssh


接下来要做的是把 id_rsa.pub 的内容添加到 GitHub 上，这样本地的 id_rsa 密钥跟 GitHub 上的 id_rsa.pub 公钥进行配对，授权成功才可以提交代码。


GitHub上添加SSH Key
首先在 GitHub 上的设置页面，点击最左侧 SSH and GPG keys ：
然后点击右上角的 New SSH key 按钮：


需要做的只是在 Key 那栏把 id_rsa.pub 公钥文件里的内容复制粘贴进去就可以了（上述示例为了安全粘贴的公钥是无效的），Title 栏不需要填写，点击 Add SSH key 按钮就ok了。












To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
