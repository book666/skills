# git软件的使用

## 从GitHub向本地down文件

#### 方法一：

步骤1：获取GitHub中的代码仓库的SSH  
步骤2：在本地打开一个文件夹，点击右键，选择Git Bash Here  
步骤3：在指令中输入：”git clone ‘代码仓库的SSH地址’“命令行，达到100%，下载成功  
如: git clone git@github.com:book666/book1.git

#### 方法二：

步骤1：在本地一个文件夹, 点击右键，打开Git Gui，点击Clone Existing Repository  
步骤2：输入Source Location 和 Target Directory，点击ok；  
Source Location 形如: https://github.com/abc/cde.git 或 git@github.com:abc/cde.git  
Target Directory 形如: cde  

注意：Target Directory选则的文件夹是未创建的，工具会自动创建。直接输入"abc",则在本地当前文件夹下创建"abc"目录.

## 使用git GUI进行Push操作
步骤1：修改属性配置-改为utf-8. 在图形窗口 (Git Gui) , 选择 Edit-->Options, 在里面修改。  
步骤2：选择中下部的按钮"Rescan", 然后选择"Stage Changed", 然后选择"Commit", 然后选择"Push", ok。

如果使用git过程中出现 "please tell me who you are"，需要设置一下使用者的身份。  
在命令行窗口 (Git Bash) , 输入以下:
```  
git config user.name "username"
git config user.email "username@XXX.com"
```
或者在图形窗口 (Git Gui) , 选择 Edit-->Options, 在User Name和Email Address中输入相应值就好。
