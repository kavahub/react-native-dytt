# react-native-dytt

[![Gitee stars](https://gitee.com/pinweiwan/react-native-dytt/badge/star.svg)](https://gitee.com/dromara/react-native-dytt/stargazers)
[![Gitee forks](https://gitee.com/pinweiwan/react-native-dytt/badge/fork.svg)](https://gitee.com/dromara/react-native-dytt/members)
[![License](https://img.shields.io/github/license/kavahub/react-native-dytt.svg)](https://github.com/kavahub/react-native-dytt/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/kavahub/react-native-dytt?style=flat-square&logo=GitHub)](https://github.com/kavahub/react-native-dytt/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/kavahub/react-native-dytt?style=flat-square&logo=GitHub)](https://github.com/kavahub/react-native-dytt/network/members)
[![GitHub watchers](https://img.shields.io/github/watchers/kavahub/react-native-dytt?style=flat-square&logo=GitHub)](https://github.com/kavahub/react-native-dytt/watchers)
[![GitHub release](https://img.shields.io/github/release/kavahub/react-native-dytt?style=flat-square&logo=GitHub?color=blu)](https://github.com/kavahub/react-native-dytt/releases)

[Gitee](https://gitee.com/pinweiwan/react-native-dytt)
[GitHub](https://github.com/kavahub/react-native-dytt)

#### 环境

```text
Windows 10
Nodejs v14.17.0
npm 6.14.13
```

#### 如何运行

修改源，使用ali云：

```text
npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```
安装插件：

安装插件

```text
npm install -g react-native-cli
```

克隆代码到本地，首先install

```text
npm install
```

使用USB连接手机，手机设置开发模式。运行命令安装：

```text
npx react-native run-android
```

#### FAQ

Q:

```text
运行React Native Tools出现错误
Invalid regular expression: /(.*\\__fixtures__\\.*|node_modules[\\\]react[\\\]dist[\\\].*|website\\node_modules\\.*|heapCapture\\bundle\.js|.*\\__tests__\\.*)$/: Unterminated character class
```

A:

```text
nodejs版本高,修改 ./node_modules/metro-config/src/defaults/blacklist.js
/node_modules[/\\]react[/\\]dist[/\\].*/,
改为
/node_modules[\/\\]react[\/\\]dist[\/\\].*/,
```

Q:

```text
编译并运行时出现错误
Scanning folders for symlinks in C:\Users\wpw\workspace\eac-mobile\node_modules (26ms)
Starting JS server...
Building and installing the app on the device (cd android && gradlew.bat installDebug)...

FAILURE: Build failed with an exception.

* What went wrong:
Could not determine java version from '11.0.5'.
```

A:

```text
JDK必须用1.8版本
```

Q:

```text
make sure your bundle is packaged correctly or you're running a packager server
```

A:

```text
在项目目录运行：
react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle
```

#### 其他开源项目

- [DYTT](https://github.com/XboxYan/DYTT) : 第三方电影天堂React Native客户端V2.0


#### 参考文档

- [React Native 中文网 - 打包发布](https://reactnative.cn/docs/signed-apk-android)

# 更新记录

#### 20211115

使用 [360看看](https://m.kkw361.com) 数据源


