# XMiPushEnhance

一个欺骗应用让他们误以为设备是小米的 Xposed 插件。

## 使用

1. 去 [Releases](https://github.com/MiPushFramework/XMiPushEnhance/releases) 下载最新 APK。

2. 安装并激活模块。

3. 重启。

### 迁移

这个模块是由原推送服务中的 Xposed 模块迁移来的。迁移过程中保留了原核心功能，但去掉了自定义欺骗哪些软件的设置。这个功能可以通过 EdXposed 的应用白名单功能实现。如果您没有在使用 EdXposed，那么它将会自动欺骗所有软件，黑名单中的除外。

## 原理

由于部分应用带有多个推送服务，它们有时会在小米设备上启用小米推送。这个模块有助于欺骗他们。

## 内置黑名单

为了防止出现意外情况，模块内置了一组黑名单。包名等于或近似于黑名单中的软件将不被欺骗。没有选项可以关闭或修改黑名单。这些软件通常包括系统关键组件和依赖于机型判断的软件（如相机）。如果您对黑名单有建议，可以通过 Issue、Pull Request 等方式贡献。

# License

GPL v2
