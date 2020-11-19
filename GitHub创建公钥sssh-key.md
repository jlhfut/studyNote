## 本地ssh-key的创建

默认已经装好了git,如果没有安装的话，请百度如何安装

在命令行中输入下面命令
 `ssh-keygen -t rsa -C "你的邮箱地址"`

如果提示找不到ssh-keygen 这个命令的话,请检查是否有安装git 以及是否要ssh-keygen加入环境变量
 然后直接回车三连（三次回车）



![img](https:////upload-images.jianshu.io/upload_images/2087032-5253a1b7bfd23f2c.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/611)

image

然后 li* mac 等系统的同学 直接输入
 `cat ~/.ssh/id_rsa.pub` 然后直接复制里面的所有的内容

windows的同学,打开当前计算机名（如我当前计算机名是 `kimga`
 `C:\Users\kimga\.ssh`下面的`id_rsa.pub`,然后复制里面的所有内容

![img](https:////upload-images.jianshu.io/upload_images/2087032-7073feda795b6fde.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/394)

image



## github 设置

1. 打开github[设置ssh-key的地址](https://github.com/settings/ssh/new)

2. 在title里面输入你这个key用在哪的,(可以随便写)

3. 在key里面粘贴进去上面复制的

4. ![img](https:////upload-images.jianshu.io/upload_images/2087032-1ba7dd2ddd5136bc.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/785)

   image

5. 点击add ssh key，然后输入GitHub密码就好了

## 测试

在命令行输入
 `ssh -T git@github.com`
 会有一个警告,直接输入`yes`
 然后会看到 `Hi xxx! You've successfully authenticated, but GitHub does not provide shell access.`
 则成功了

![img](https:////upload-images.jianshu.io/upload_images/2087032-e1dc2d9d98b628de.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/721)



作者：高金01
链接：https://www.jianshu.com/p/26cda3d42943
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。