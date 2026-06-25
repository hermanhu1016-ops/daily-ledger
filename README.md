# 日常记账 Android 项目

这是标准 Android Studio 工程，用原生 WebView 打开记账页面。

## 生成 APK

1. 用 Android Studio 打开 `DailyLedgerAndroid` 文件夹。
2. 等待项目同步完成。
3. 点击菜单 `Build` -> `Build Bundle(s) / APK(s)` -> `Build APK(s)`。
4. 生成的 APK 通常在 `app/build/outputs/apk/debug/app-debug.apk`。
5. 把这个 APK 发送到安卓手机安装。

## 为什么改成这个方式

前面几个 APK 是在没有 Android SDK 的环境里手工拼出来的，虽然能安装，但你的手机启动时会闪退。这个工程会交给 Android 官方工具链生成清单、DEX 和签名，可靠性高得多。
