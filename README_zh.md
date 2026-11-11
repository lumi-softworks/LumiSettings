# LumiSettings

📖 [中文版](README_zh.md) | [English](README.md)

Coffic 应用共享的设置 provider 契约与 SwiftUI 导航。

`ProviderSettingView` 提供：

- `SettingViewProviding` 与 `DefaultSettingViewProviding`：注册设置条目。
- 使用 LumiUI 样式的共享 macOS 设置侧边栏与详情外壳。
- `IOSSettingsNavigationView`：iOS 设置导航。应用宿主在自己的窗口或 sheet 中展示它。
- `ProjectDetailSectionItem`：插件贡献的设置分区。

添加包与 product 依赖：

```swift
.package(url: "https://github.com/lumi-softworks/LumiSettings.git", from: "1.0.0")
```

```swift
.product(name: "ProviderSettingView", package: "LumiSettings")
```

本包依赖 [LumiUI](https://github.com/lumi-softworks/LumiUI) 提供共享视觉组件。
窗口创建、应用导航栏与应用专属设置页面仍留在宿主应用中。
