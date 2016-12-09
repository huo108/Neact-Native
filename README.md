# Neact-Native
neact-native学习日记

## 1.搭建开发环境（mac）
### Homebrew安装
   在终端或iterm2运行：

     /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"


 译注：在Max OS X 10.11（El Capitan)版本中，homebrew在安装软件时可能会碰到/usr/local目录不可写的权限问题。可以使用下面的命令修复：

    sudo chown -R `whoami` /usr/local
 
 
 ### Node（4.0以上版本）

    brew install node

安装完node后设置npm镜像以加速后面的过程（或使用科学上网工具）。

    npm config set registry https://registry.npm.taobao.org --global

    npm config set disturl https://npm.taobao.org/dist --global

### React Native的命令行工具（react-native-cli）

React Native的命令行工具用于执行创建、初始化、更新项目、运行打包服务（packager）等任务。

    npm install -g react-native-cli   (-g :全局)

如果出现EACCES: permission denied这样的权限报错，需要修复/usr/local目录的所有权：

    sudo chown -R `whoami` /usr/local

### JDK(1.8以上版本)

[下载地址](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
安装完后运行

    javac -version 检查是否安装成功！

### Android Studio(2.0以上版本)

Android Studio包含了运行和测试React Native应用所需的Android SDK和模拟器。

安装完成后下载必须的SDK：

- 在SDK Platforms窗口中，选择Show Package Details，然后在Android 6.0 (Marshmallow)中勾选Google APIs、Intel x86 Atom System Image、Intel x86 Atom_64 System Image以及Google APIs Intel x86 Atom_64 System Image。

![](https://github.com/huo108/Neact-Native/blob/master/imgs/android-sdk-build-tools.png)

在SDK Tools窗口中，选择Show Package Details，然后在Android SDK Build Tools中勾选Android SDK Build-Tools 23.0.1。（必须是这个版本）

![](https://github.com/huo108/Neact-Native/blob/master/imgs/android-sdk-platforms.png)




