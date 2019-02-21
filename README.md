# change-remote
改变git项目远程地址

学习资源：https://blog.csdn.net/m0_37034294/article/details/79986198

怎么更换git远程仓库地址
方法一 ： 通过命令直接修改远程仓库地址

git remote 查看所有远程仓库
git remote xxx 查看指定远程仓库地址
git remote set-url origin 你新的远程仓库地址

方法二： 先删除在添加你的远程仓库

git remote rm origin
git remote add origin 你的新远程仓库地址

方法三： 直接修改你本地的.git文件

这里需要注意的问题是需要进入你的项目目录中
例如：你的项目名为test，那么你就进入test文件夹。
**.git文件是隐藏文件你需要显示隐藏文件才能看见**

进入.git文件编辑.git文件中的config文件修改config文件中的url路径为你的新远程仓库地址路径。
