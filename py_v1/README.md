# 微博批量拉黑脚本 V1

## 安装
### 1. 下载
![download](../imgs/download.png)

### 2. 安装 Python
[Python 3.6.3](https://www.python.org/downloads/release/python-363/)
选择对应版本安装

### 3. 安装 Fiddler
[官网](http://www.telerik.com/fiddler)

也可以 360软件管家 直接搜索安装

## 运行
1. 打开 Fiddler

2. 打开 [微博监督员关注列表](http://weibo.com/p/1006066264005608/follow?page=1)， 选择一个没有拉黑的用户，按照如下方法拉黑:
+ 鼠标停留在 ID 上方
+ 在弹出的小窗口中拉黑

![blcak](../imgs/black.png)

3. 如下图所示，在 Fiddler 中选中对应请求，选择 Raw 格式进行查看，并将结果复制到 http.txt 中。

![fiddler](../imgs/fiddler.png)

4. 在当前文件夹打开命令行，执行 `python run.py`, 或者直接双击 `run.bat` ， 就能拉黑 list.txt 中的所有用户。



## 问题
其实我是 Python 小白，感觉 `request.urlopen` 慢的不可思议。

最开始我是拿 Matlab + java.swing.Robot + Fiddler 模拟输入干的。
