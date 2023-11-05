# 考试倒计时
基于python，调用tkinter、time
如果你想把它生成exe可执行文件，请按照下面的步骤进行。

## 1、安装pycharm（如果你有可以跳过）

[website](https://www.jetbrains.com/pycharm/download/#section=windows)


## 2、在pycharm中打开“terminal”

## 3、输入：

```
pip install pyinstaller
```
```
中国大陆用户使用豆瓣源： pip install pyinstaller -i https://pypi.douban.com/simple/
```

## 4、打包：

```
基本用法：
1.简单打包

# -D，--onedir创建包含可执行文件的单文件夹包（默认）
pyinstaller *.py

2.打包为单个*.exe文件

# -F， - onefile创建一个文件捆绑的可执行文件。
pyinstaller -F *.py

3.使打包后的EXE文件不带小黑框

# -c 打开标准i/o控制台窗口（默认）
# -w 无标准i/o控制台窗口
pyinstaller -w *.py

4.多个*.py文件同时打包

pyinstaller main.py -p other-1.py -p other-2.py

5.添加资源文件

1）把所有的文件都放在一个文件夹里面。

2）执行：

pyinstaller --clean -F callMain.py --add-binary=D:\WinPyQt5.9-32bit-3.5.3.1\PyQt5-codes\pack\yundamaAPI.dll;''
6.添加图标

pyinstaller *.py -i **.ico
```
```
pyinstaller -w main.py
```

## 5、找到它：
他总是被打包在项目下的“dist”文件夹。
