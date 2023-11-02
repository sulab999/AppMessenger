# AppMessenger(appmsg)

下载地址：https://github.com/sulab999/AppMessenger/releases/download/v4.6.3/appmsg4.6.3.zip


# 介绍
## 解析APP  
一款适用于以APP病毒分析、APP漏洞挖掘、APP开发、HW行动/红队/渗透测试团队为场景的移动端(Android、iOS)辅助分析工具，可以帮助APP开发工程师、病毒分析师、漏洞/安全研究员提高工作效率，帮助渗透测试工程师、攻击队成员/红队成员快速收集到移动端中关键的资产信息并提供基本的信息输出,如：包名（packageName）、版本(versionName\versionCode)、应用签名(Signature)、文件MD5、SDK、URL、APP漏洞等信息。  

## APK文件解析  
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/pic1.png" width="500px">
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/pic2.png" width="500px">
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/pic3.png" width="500px">

## IPA文件解析  
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/ipa1.png" width="500px">
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/ipa2.png" width="500px">

## 高级检测(目前只支持APK)  
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/gj1.png" width="500px">
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/gj2.png" width="500px">
<img src="https://github.com/sulab999/AppMessenger/blob/master/pic/gj3.png" width="500px">
# 前言
- 本项目始于SULAB安全团队，并联合知识星球：移动安全
- 如果您觉得这个项目对您有用，请点击本项目右上角的"star"按钮。
- 如果您想持续跟进新的版本情况，请点击本项目右上角的"Watch"按钮。
- 会在知识星球发布内测或特别版
- 新的功能或者需求会持续进行开发，欢迎提BUG。
- 后期更新版本见releases


# 适用场景
- APP病毒分析
- APP漏洞挖掘
- APP信息收集
- 日常渗透测试/攻防演练中对APP中涉及的关键资产信息收集，比如URL地址、IP地址、关键字等信息的采集等。

# 功能介绍:
- [√] 支持任意文件MD5识别
- [√] 支持DEX、APK、IPA文件的信息收集
- [√] 支持Android壳识别（识别准确率99%，业界一流）
- [√] 支持基础检测：文件路径、包名、版本名、文件MD5、文件SHA1、DEX MD5、文件大小、allowbackup、debuggable、打包时间
- [√] 支持解析APP权限信息、签名信息、支持系统版本等其他信息
- [√] 支持敏感信息检测，如：url、ip等
- [√] 支持Windows系统、MacOS系统、*nux系列的系统
- [√] APP漏洞检测
- [×] 一键对APK文件重打包


# 环境说明
- App文件解析需要使用JAVA环境,JAVA版本11及以上
- Pro版已集成java环境可开箱即用

# 使用方法
1、如有java环境，可双击apkmsg.jar，即可启动，直接将APP拖入即可自动识别  
2、如果无法打开或显示有乱码，可下载配套的jdk11，运行里面写好的脚本，即可一键启动  
3、MAC和Linux系统需要对运行脚本和JAVA_HOME里的文件授予可执行权限，命令如下  
chmod 777 运行mac/运行linux.sh  
chmod -R 777 JAVA_HOME   
jdk11：https://github.com/sulab999/AppMessenger/releases/download/v4.6.2/jdk11.zip  
![start](https://github.com/sulab999/AppMessenger/blob/master/pic/start.png)   

# 感谢“移动安全”知识星球的小伙伴，欢迎加入
![zsxq](https://github.com/sulab999/AppMessenger/blob/master/pic/jqr.jpeg)
# 不温不火的公众号  
![webchat](https://github.com/sulab999/Taichi/blob/main/webchat.png)  
# 免责声明
请勿将本项目技术或代码应用在恶意软件制作、软件著作权/知识产权盗取或不当牟利等非法用途中。实施上述行为或利用本项目对非自己著作权所有的程序进行数据嗅探将涉嫌违反《中华人民共和国刑法》第二百一十七条、第二百八十六条，《中华人民共和国网络安全法》《中华人民共和国计算机软件保护条例》等法律规定。本项目提及的技术仅可用于私人学习测试等合法场景中，任何不当利用该技术所造成的刑事、民事责任均与本项目作者无关。

# 历史更新记录
v4.6更新的功能：  
1、增加SDK检测  
2、优化加固特征  
3、优化任意文件md5检测  

v4.5.1更新的功能：  
1、增加allowBackup和debuggable检测  
 
v4.5更新的功能：  
1、优化代码结构，采用不依赖aapt方案  
2、基于java11编译，优化java9读取打包时间出错的bug  

v4.4.1更新的功能：  
1.优化证书解析，支持DSA证书类型 

v4.4更新的功能：  
1.支持mac系统，针对mac系统进行了相关优化(Mac系统需要chmod 777 aapt) 

v4.3更新的功能：  
1.增加新的加固特征 

v4.2更新的功能：  
1.优化加固特征 

v4.1更新的功能：  
1.加入了更新机制  

v4.0更新的功能：  
1.支持解析ipa文件  

v3.4更新的功能：  
1.支持解析任意文件md5和sha1  

v3.3更新的功能：  
1.优化读取文件越界问题  
2.优化证书MD5匹配  
3.不依赖keytool解析签名  

v3.2更新的功能：  
1.更新加固特征  
2.更新权限特征  
3.增加二级md5解析  
4.文件大小以字节显示  
