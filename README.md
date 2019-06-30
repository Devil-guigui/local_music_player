# 本地音乐播放器

### 具体思路

使用python制作一个本地的音乐播放器，通过tkinter库编写音乐播放器的界面，使用eyeD3库来处理MP3文件，获取歌曲的时长。打开本地音频文件添加到歌曲列表，然后有播放、停止和暂停功能，还可以选择上一曲和下一曲，可以通过滑块进行音量控制。

### 模块准备

安装tkinter模块

安装eyeD3模块



#### 注意事项：

编译遇到错误“failed to find libmagic. Check your installation” ，在https://pypi.org/project/python-magic-bin/#files下载[python_magic_bin-0.4.14-py2.py3-none-win_amd64.whl](https://files.pythonhosted.org/packages/07/c2/094e3d62b906d952537196603a23aec4bcd7c6126bf80eb14e6f9f4be3a2/python_magic_bin-0.4.14-py2.py3-none-win_amd64.whl)(下载对应安装包)到  C:\Users\administor  ，然后cmd运行pip install python_magic_bin-0.4.14-py2.py3-none-win_amd64.whl以解决错误

如果遇到PhotoImage报错： couldn't recognize data in image file，需要用格式工厂转换成gif图片，PhotoImage不是看图片后缀名，而是图片本身的类型。

如果遇到错误“name 'filedialog' is not defined”，需要在前面加上from tkinter import filedialog（单独淡入？）或者import tkinter as tk