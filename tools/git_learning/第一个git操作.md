# 一个简单的git使用流程示例
## 第一步：下载git
使用命令：*$ sudo apt-get install git*
## 第二步：在一个目录下创建git仓库
使用命令：*$ git init*
## 第三步：添加想要上传的文件
使用命令：*$ git add '需要上传的文件'* **这个文件一般是会被改动的；git add本质上是将该文件放入暂存区**
## 第四步：提交代码并给出声明
使用命令：*$ git commit -m '提交说明,比如说增加了统计功能'* **使用git commit提交并创建版本**
以上是一个简单的本地仓库用git进行版本控制的示例

# 与github联动
如何将本地代码推送到github上？
## 第一步：创建一个仓库，点击绿色标志：new repository，里面需要填写仓库名等信息。建议与本地仓库名称一致。
## 第二步：关联远程仓库
使用命令：*$ git remote add origin git@github.com:timesall/bookstore.git* **这里的ssh key仅做示例，具体以自己的为主**
## 第三步：将文件推送到github
使用命令：*$ git push -u origin master* **-u参数是将master所有分支上传到github上，以后就不用加上-u参数了**

**其中origin是远程仓库的别名（默认名称）。**
当你 git clone 一个仓库时，Git 会自动将你克隆的那个远程仓库命名为 origin。
它本质上是一个URL 的缩写，指向远程服务器上的仓库地址（如 GitHub 上的项目）。
你可以用 git remote -v 查看 origin 对应的实际地址。
当然你也可以添加其他远程仓库并起别的名字（如 upstream），但 origin 是最常用的默认名字。
**master是本地分支的名字**
表示你当前要推送的本地分支名叫 master。
对于较旧的 Git 项目，默认主分支名是 master；较新的项目（2020年后）默认主分支名常为 main，此时命令会变成 git push -u origin main。
它的作用是指定从本地的哪一个分支推送到远程。