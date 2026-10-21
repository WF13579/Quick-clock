# Quick-clock（一键锁屏）

一个极简的 Android 一键锁屏小程序：点击图标 → 首次使用授予设备管理员权限 → 立即锁屏。

## 使用方法

1. 安装 APK 后打开应用；
2. 首次运行会弹出「激活设备管理员」界面，点击激活（仅使用锁屏权限，可随时在系统设置中撤销）；
3. 之后每次点开应用即可立即锁屏。

## 构建

```bash
gradle assembleDebug   # 或用 Android Studio 直接打开
```

也可通过 GitHub Actions 自动构建（`.github/workflows/build.yml`），在仓库 Actions 页面下载 APK。

## 技术

- Kotlin + DevicePolicyManager（`lockNow()`）
- minSdk 21 / targetSdk 34
