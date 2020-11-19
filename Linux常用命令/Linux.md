## Linux常用命令

* cd:改变目录
* cd.. :回退到上一个目录，直接cd进入到默认目录
* pwd:显示当前所在的目录路径
* ls(ll):都是列出当前目录中的所有文件，们只不过ll列出的内容更为详细
* touch:新建一个文件 如 touch index.js 就会在当前目录下新建一个index.js文件
* rm:删除一个文件，rm index.js就回吧index.js文件删除
* mkdir:新建一个目录，就是新建一个文件夹
* rm -r：删除一个文件夹，rm -r -src 删除src目录
* mv ：移动文件夹，mv index.js src index.js 是我们要移动的文件，src是目标文件夹
* rest：重新初始化终端/清屏
* clear：清屏
* history:查看命令历史
* help:帮助
* exit:退出
* #：表示注释

### Git 配置

查看配置 git config -l

设置用户名与邮箱（用户名标识，必要）

git config --global user.name "liujing" #名称

git config --global user.email 1113076429@qq.com #邮箱

* 查看不同级别的配置文件

  #查看系统config

  git config --system  --list

  #查看当前用户（global）配置

  git config --global --list

  ** Git相关配置文件

  1）Git\mingw64\etc\gitconfig：Git安装目录下的gitconfig   ---system系统级

  2）C:\User\Administrator\.gitconfig 只适用于当前登录用户的配置 ---global 全局

  

  ## Git 基本理论（核心）

  **工作区域 **

  ​	Git本地有三个工作区域：工作目录（Working Directory)、暂存区（Stage/Index)、资源库（Repository或Git Directory）。如果加上远程的Git仓库（Remote Directory)就可以分为4个工作区域。文件在这四个区域之间的转换关系如下：

  

  ![image-20201119093711404](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20201119093711404.png)

* Workspace：工作区，就是您平时存放项目代码的地方
* Index/Stage：暂存区，用于临时存放你的改动，事实上他只是一个文件，保存即将提交到文件列表信息
* Repository：仓库区（或本地仓库），就是安全存放数据的位置，这里有你提交的所有版本数据。其中HEAD指向最新放入仓库的版本。
* 





