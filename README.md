# m3u8_downloader_4_yingke
## 映客m3u8格式历史直播记录下载器
## 目前已经实现ffmpeg合并视频片段，程序已更新
![demo_gif](/img/demo4python.gif)

网址分析
------------
[项目demo测试的映客页面传送门](http://www.inke.cn/live.html?uid=3677006&id=1481727812972630)

http://www.inke.cn/live.html?uid=3677006&id=1481727812972630

另一种
https://mlive15.inke.cn/app/hot/record?uid=163155224&liveid=1501310503474850&ctime=1501310503&share_uid=80864215&share_time=1512714655&share_from=

需要人为提取的房间id即为网址中的id=后面那串数字，在本例中为1481727812972630

另一种需要提取的是liveid，在本例中为1501310503474850
## 注意！
本示例地址中的id可能会失效，由于未知的原因，示例视频的id可能会改变，但直接浏览器访问没有异常，请自己随便找个其他录播地址测试！

目前实现的功能 : )
------------
- 下载映客m3u8格式的历史直播记录ts片段
- 支持根据映客房间id自动下载m3u8文件
- 支持直接读取映客m3u8文件下载
- 以二进制方式自动合并ts片段
- ts片段成功合并后自动清除缓存

###### 备注：由于每个人的系统设置不同，自动清除缓存的功能在某些计算机上可能会失败，通常的原因可能是遇到了权限问题，可尝试使用管理员身份运行

环境要求
------------
- Python 2.7（小白不作要求）

###### 备注：Python 3 理论上支持，但并未测试，欢迎反馈！


使用方法
------------

#### 方法一（Python 2.7 下工作）
Windows 10为例

开始——右键——命令提示符（管理员）

cd 切换到Python程序的目录

输入命令 python main.py

根据命令提示进行操作

###### 备注：使用前需要配置Python环境，建议使用Anaconda
###### 友情链接：获取最新Anaconda下载信息 [传送门](https://www.continuum.io/downloads)

#### 方法二（CMD 下工作）【小白推荐】
Windows 10为例

开始——右键——命令提示符（管理员）

cd 切换到exe4windows文件夹的目录

输入命令 main.exe

根据命令提示进行操作

未来可能更新的地方
----------
- 支持录制实时的直播信号
- 实现对ts片段进行mp4格式转换
- 实现对ts片段更精细的拼接（从本人的能力来看，暂时不太现实，哈哈）

demo工作示意图
-----------

#### Python 2.7 下工作（花费72秒）
![demo_gif](/img/demo4python.gif)

#### CMD 下工作（花费148秒）
![demo_gif](/img/demo4cmd.gif)

更新日志
-----------
201701209 更新 v0.21
- 优化选择m3u8文件逻辑问题

201701209 更新 v0.2
- 添加ffmpg合并

201701013 创建 v0.1
- 框架预览版

交流讨论
----------
- QQ: 691066230
- email: admin@xyf.im
