# RSA密钥的生成与转换


### key的生成

* 在linux系统下，通过 ssh-keygen 命令生成。  
生成的文件在目录 ~/.ssh/ 下，2个文件，id_rsa 和 id_rsa.pub 。

* 在windows系统下，通过PuTTyGen程序生成。  
key生成后，通过点击“Save private key”输出ppk文件，这是putty使用的key文件，其他软件无法使用。  
可点击Conversions下拉菜单，选中Export OpenSSH key，输出OpenSSH key-gen格式的key。

* 网上很多在线生成RSA密钥对的，如 `http://web.chacuo.net/netrsakeypair`

### key的转换

#### 从PuTTyGen生成的private key转换成OpenSSH key-gen的key。

打开PuttyGen软件，点击load按钮，导入puttygen的private key。点击Conversions下拉菜单，选中Export OpenSSH key。输入要保存的文件名，例如id_rsa。这就是OpenSSH key-gen的key。

#### 从OpenSSH key-gen的key转换成PuTTyGen生成的private key。

打开PuttyGen软件，点击Conversions下拉菜单，选中Import key，导入OpenSSH key-gen的private key。点击“Save private key”即生成 ppk 文件。
