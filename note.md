# Vue-admin

> **这是一个从零到一的Vue后台管理系统项目** 
>
> 1. 创建仓库
> 2. 配置项目



### 一、创建仓库配置github

+ 拷贝项目到本地

  ```git
  git clone https://github.com/lingzhi42166/vue-admin.git
  ```

+ 创建分支

  一般开发项目都不会在主分支上开发，并且多人协作的时候，都会创建自己的分支，最终再合并在一个分支上。

  ```git
  git branch --list                   => 查看分支列表 *后为当前分支   默认是master 主分支
  git branch dev                      => 创建dev分支
  git checkout dev   	                => 切换到dev分支
  git push --set-upstream origin dev  => 发布分支  前面的创建分支 只是作用在工作区 远程仓库并没有 
  命令扩展:
  	git checkout -b <name>                => 创建并切换到该分支
  	git branch -d your_branch             => 删除本地分支
  	git push origin --delete your_branch  => 删除远程分支
  建议:
  	建议直接使用VScode快捷操作git 教程请看vscode-git
  ```

  > **分支知识点**
  >
  > + 分支是就是科幻电影里面的平行宇宙，当你正在电脑前努力学习Git的时候，另一个你正在另一个平行宇宙里努力学习SVN。如果两个平行宇宙互不干扰。
  >
  > + master: 主分支(仓库自带的) 在实际的项目开发中，一般不会在主分支上开发的
  >
  > + dev: 开发分支(自己创建的)     一般再此分支上开发项目
  >
  >   + 版本分支:
  >
  >     建立在dev分支下(分支A下创建新的分支B，是指B使用A分支下的代码(因为更新都是在原有基础上的)，并不是层级关系) 。该分支是用来管理不同的版本的，一个版本一个分支
  >
  >     feature-vue-admin-V1.0.0-20200614 分支完整名称
  >
  >     ​	feature: 描述当前分支类型
  >
  >     ​	vueAdmin: 项目名称
  >
  >     ​	V1.0.0: 版本号
  >
  >     ​	20200614: 分支建立日期
  >
  >   + BUG分支
  >
  >     具体还不会应用到 pass 
  >
  >     

  ***

  切换分支后，可以重新打开gitbash，将会看到当前工作区的分支为dev，所以在不切换分支的情况下，所有的文件推送都是推送到dev分支上(在VScode中提交可以看到)，如果一个项目是多人协作开发的，一般都会有自己的分支，**互不影响（推送到dev分支后，在github中可以看到两个分支，其中我们修改的文件在master分支中式看不到修改的内容的），最后再合并到一个分支上**

  ![image-20200614211122944](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200614211122944.png)

