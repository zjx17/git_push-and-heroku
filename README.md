# git_push-and-heroku
## git_push
下来我要检测我的Ubuntu系统中有没有安装Git。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/1.png)

返回这么一大串就表示已经安装了。如果没有安装就使用语句。

现在开始我们的git命令操作。

第一步、通过git init命令把这个目录变成Git可以管理的仓库。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/3.png)

第二步、将文件添加到版本库中。这里会涉及到几个指令：

git add file  //添加指定的文件

git status   //查看版本库当前的状态。

git commit  //提交文件到仓库中

注意，由于我们添加的是整个文件，所以使用git add file命令就比较麻烦。这里我是使用

git add .   (.表示文件夹下的所有的文件) 

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/4.png)

使用git status查看当前的信息就是在master分支上，并且初始化了commit命令，等待提交。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/5.png)

commit后面的 -m表示可以添加描述。到这里就已经提交文件到本地仓库了。

第三步、登陆github的官网，注册自己的github账户。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/6.png)

由于你的本地Git仓库和GitHub仓库之间的传输是通过SSH加密的，所以需要设置SSH keys。这里我推荐一篇文章讲的非常的详细。

http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001374385852170d9c7adf13c30429b9660d0eb689dd43a000

我假设在看完我推荐的文章之后，你已经成功的设置好了SSH keys。接下来的步骤就是在gitHub中添加仓库和添加文件到远程库了。


第四步、在gitHub中添加仓库

首先测试一下，SSH密钥是否配置好。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/8.png)

如果配置好，会有上图的返回。

接下来在github中新建一个仓库。取名Java_src_learning。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/9.png)

设置仓库名和相关的属性。(取消Readme容易Push)

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/10.png)

第五步：添加文件到远程库。使用指令如下：

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/12.png)

然后使用git push指令来完成上传。

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/13.png)

第六步、查看项目文件是否成功的添加

![image](https://github.com/zjx17/git_push-and-heroku/blob/master/picture/16.png)

<br>引自 http://blog.csdn.net/lulei1217/article/details/51137906</br>
