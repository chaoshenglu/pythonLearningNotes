## 第1课 Python的环境配置（Windows）

# 1.安装python2.7
[python2.7 64位 下载地址](https://www.python.org/ftp/python/2.7.14/python-2.7.14.amd64.msi)

# 2.配置python2.7的环境变量
我的电脑-属性-高级系统设置-环境变量-系统变量-Path 
填写或追加python2.7的安装地址即可

详细步骤可参考：[链接](https://jingyan.baidu.com/article/48206aeafdcf2a216ad6b316.html)

# 2.安装sublime test 3
[sublime test 3 64位 下载地址](https://download.sublimetext.com/Sublime%20Text%20Build%203143%20x64%20Setup.exe)

# 3.sublime test 3 汉化
[汉化包 下载地址](https://pan.baidu.com/s/1sliHXBf)

使用方法：将此汉化包放在软件安装目录下“Installed Packages”文件夹中。

“Installed Packages”的上级目录一般是AppData/Roaming/Sublime Text 3。

# 4.使用sublime test 3 编译python代码
sublime test 3 - 菜单 - 工具 - 编译系统 - 编译新系统

删除预置代码："shell_cmd": "make"

新增如下代码：
```
{
    "cmd": ["C:/Python27/python.exe", "-u", "$file"], 
	"file_regex": "^[ ]*File \"(…*?)\", line ([0-9]*)", 
	"selector": "source.python"
}
```

详细步骤可参考：[链接](http://blog.csdn.net/wanmeiwushang/article/details/52280357)
