# C-_QT_FAQ
C++ QT FAQ

## 1 Mac OS下的笔记
### 1.1 打包成dmg
Build Settings--Build Steps--Custom Process Step:macdeployqt my.app -verbose=1 -dmg  
Command:macdeployqt  
Arguments:my.app -verbose=1 -dmg  

## 2 Windows下的笔记
### 2.1 webenginewidgets 问题
无法找到此模块QT += webenginewidgets，需要至少在MSVC2017下编译  
### 2.2 版本属性信息
pro文件中添加   
VERSION = 0.19.1212  
QMAKE_TARGET_PRODUCT = 慧科云QT学习项目  
QMAKE_TARGET_COMPANY = 慧科教育科技集团有限公司  
QMAKE_TARGET_DESCRIPTION = 慧科云QT学习项目  
QMAKE_TARGET_COPYRIGHT = 2019 (c) Huike education technology group co. LTD  
### 2.3 中文乱码问题（Mac windows通用解决方法）
目标文件顶部加入#pragma execution_character_set("utf-8")，为了更好的跨平台，建议都是用utf-8编码。  
### 2.4 windows安装包制作工具
NSIS/VNISEdit，根据安装向导操作。



