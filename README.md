# scnu_ssp_ClockIn
今天你打卡了没？

脚本仅供学习交流，请勿用于其他用途。
  
另外脚本里细节写得不是很到位，意思到了就好。(跑

# 安装环境
python3
jdk
## 安卓打卡
安装[apk](https://github.com/wumcpq/scnu_ssp_ClockIn/releases/download/android/scnu_ssp_clockIn.apk)文件即可进行打卡  
在release中可以下载[idea工程源码](https://github.com/wumcpq/scnu_ssp_ClockIn/releases/download/android/idea.project.7z)  
需要jsoup依赖  

## browser.py
`pip install selenium`
  
`pip install tkinter`
  
安装火狐浏览器或者谷歌浏览器并且下载geckodriver放入浏览器目录下
## requsets.py
`pip install tkinter`
  
`pip install re`
  
`pip install requests`

# 初始化
## browser.py
打开browser.py并修改如下内容，即打卡内容。
```python
username = '2018213xxxx'    # 学号
password = '你的密码'       # 密码
p = 'xx省'                  # 省份
location = 'xx市xx区/县'    # 地区
```  
## requsets.py
打开requests.py并修改如下内容，即打卡内容。
```python
user = '2018xxxxx'         # 你的学号
password = 'password'      # 你的密码
area = 'xx省'              # 你的省份
location = 'xx市xx县'      # 详细位置
```
  
# 使用
## python脚本
初始化完成之后直接打开就可以愉快使用啦。  

## 安卓
填入数据即可进行打卡。  
第一次使用填入数据打卡后会保存内容，以后无需输入数据即可打卡。  
此外，apk没有做屏幕适配，测试中小米8体验良好。  
小米8实际使用效果图：  
![小米8效果图](https://github.com/wumcpq/scnu_ssp_ClockIn/raw/master/android/Snipaste_2020-05-10_18-12-27.jpg)

新增布局文件与按钮格式文件

# 自动打卡
在windows下写一个批处理文件，将改批处理文件设置开机自启动即可每天打开电脑自动打卡。
