<div align="center">

**语言版本：** [English](README.md) | [简体中文](README.zh-CN.md)

</div>

---

## ⚠️ 重要说明

本项目本体暂不开源，当前仓库主要用于发布版本和接受反馈。  
应用使用的第三方开源组件我们均已按要求公开 License。

未来会根据项目进展评估是否开放更多内容。  
感谢理解与支持！ 详细请参阅 [置顶说明](https://github.com/666OS/ClashMac/issues/15)

<br>
<p align="center">
  <img src="assets/clashmac-logo.png" alt="ClashMac Screenshot" width="300" style="filter: drop-shadow(0 4px 12px rgba(0, 0, 0, 0.15));">
</p>
<h1 align="center">ClashMac</h1>
<h3 align="center" style="margin-top: 0; margin-bottom: 20px;">轻量级 macOS Clash 菜单栏客户端</h3>

<p align="center" style="margin-top: 0; margin-bottom: 50px;">
  <a href="https://github.com/666OS/ClashMac/releases/latest">
    <img src="https://img.shields.io/github/v/release/666OS/ClashMac?style=flat-square&logo=github&color=green" alt="Latest Release">
  </a>
  <a href="https://github.com/666OS/ClashMac/releases">
    <img src="https://img.shields.io/github/downloads/666OS/ClashMac/total?style=flat-square&logo=dropbox&logoColor=white&color=gold" alt="Downloads">
  </a>
  <a href="https://t.me/Pinched666">
    <img src="https://img.shields.io/badge/Telegram-Channel-blue?style=flat-square&logo=telegram">
  </a>
</p>
<p align="center">
  <img src="assets/screenshot-cn.png" alt="ClashMac Screenshot" width="400">
</p>

## 特性

- **原生应用** - SwiftUI 开发，完美融入系统
- **轻量高效** - 菜单栏应用，资源占用低
- **网络接管** - 一键开启/关闭，系统代理&增强模式
- **特权助手** - 实现免密管理系统代理与内核
- **实时流量监控** - SSE 推送，毫秒级更新
- **可视化面板** - 流量统计、连接数、内存使用
- **Web Dashboard** - 集成控制面板访问
- **应用内更新** - 自动更新功能
- **订阅管理** - 订阅源自动更新
- **配置切换** - 多配置文件支持

## 下载

在 [Releases 页面](https://github.com/666OS/ClashMac/releases/latest) 下载最新版本：

- **Apple Silicon (M1/M2/M3/M4)**: `ClashMac-v*-macos-arm64.zip`
- **Intel Mac**: `ClashMac-v*-macos-x86_64.zip`

**兼容方案**：请参阅 [测试配置](https://github.com/666OS/YYDS/tree/main/mihomo/config)

**安装步骤**：
1. 解压下载的 zip 文件
2. 将 `ClashMac.app` 拖到"应用程序"文件夹
3. 首次打开时，右键点击并选择"打开"（绕过安全检查）

**提示**: 不确定您的 Mac 类型？点击左上角  → 关于本机，查看"芯片"信息。

> **注意：Mac Gatekeeper 可能会拦截未签名应用**  
> 因为 ClashMac 没有经过 Apple notarize（公证），macOS 默认不允许直接打开。

### 解决方法

#### 方法 1：系统设置中允许打开
1. 尝试打开 ClashMac，出现安全警告时点击"完成"
2. 打开 **系统设置** → **隐私与安全性**
3. 向下滚动，找到提示："ClashMac 已被阻止打开"
4. 点击旁边的"仍要打开"
5. 在弹出框再点击"仍要打开"即可

#### 方法 2：终端解除限制
在"终端"中输入：

```bash
xattr -cr /Applications/ClashMac.app
```
回车后重新打开应用


#### 方法 3：移除隔离属性

在"终端"中输入：
```bash
xattr -d com.apple.quarantine /Applications/ClashMac.app
```
回车后重新打开应用

## 许可证

ClashMac 是一个专有的闭源应用程序。  
本仓库仅提供二进制发布版本。

本项目使用了第三方开源组件。  
完整的许可证列表可在此处查看：

[第三方许可证](https://github.com/666OS/ClashMac/blob/main/THIRD_PARTY_LICENSES.txt) 

## 致谢

- [mihomo](https://github.com/MetaCubeX/mihomo)
- [Vernesong](https://github.com/vernesong/mihomo)
- [Zashboard](https://github.com/Zephyruso/zashboard)

## Star History
[![Star History Chart](https://api.star-history.com/svg?repos=666OS/ClashMac&type=Date)](https://star-history.com/#666OS/ClashMac&Date)

---

<p align="center">
  Made with ❤️ for macOS
</p>
