# Ghostty 配置：现代、极简、低延迟终端体验

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/SiliconAwakening/ghostty-config/main/pic-1.jpg" width="400" alt="Theme Preview"></td>
    <td><img src="https://raw.githubusercontent.com/SiliconAwakening/ghostty-config/main/pic-2.jpg" width="400" alt="Quick Terminal"></td>
  </tr>
</table>

一个干净、快速、macOS 友好的 [Ghostty](https://github.com/ghostty-org/ghostty) 配置文件，融合了：

- **支持 MAC/Vim 风格** 的分屏导航（cmd/ctrl+h/j/k/l）
- **Catppuccin Mocha** 主题 + JetBrains Mono 字体
- 优雅的毛玻璃背景（macOS glass-clear）
- 轻量透明 + 现代视觉微调
- 安全的剪贴板保护 + zsh shell integration
- 超大回滚缓冲（2000万行）

适合追求低延迟、视觉舒适的开发者。

## 特性亮点

- **字体**：JetBrains Mono + 连字支持（calt & liga），14pt 加粗优化
- **主题**：Catppuccin Mocha（深色优雅）
- **透明 & 毛玻璃**：背景透明 0.7 + macOS glass-clear 效果
- **分屏导航**：支持MAC/Vim 风格
- **macOS 优化**：透明标题栏、非原生全屏、命令执行完毕通知
- **安全**：粘贴保护 + bracketed paste 安全模式
- **实用**：选中即复制到剪贴板、输入时隐藏鼠标、快速下拉终端（Quake 风格）

## 安装

1. 确保已安装 Ghostty（目前仅 macOS，支持 brew / 手动下载）

   ```bash
   brew install --cask ghostty
   ```
2. 创建或覆盖配置文件：
   ```bash
   mkdir -p ~/.config/ghostty
   curl -o ~/.config/ghostty/config https://raw.githubusercontent.com/SiliconAwakening/ghostty-config/main/config.ghostty
   ```


 或者直接复制下面的完整配置内容到 `~/.config/ghostty/config`

3.重启 Ghostty 或按 `Cmd + Shift + ,` 重载配置

## 常见问题

Q：为什么分屏后字体看起来有点挤？

A：adjust-cell-height = 5% 已经做了轻微拉伸。如果仍不满意，可调到 8%~12%。

Q：毛玻璃效果不生效？

A：确保 macOS ≥ 14，且 background-blur = macos-glass-clear（或试试 macos-glass-regular）。


## 致谢
- Ghostty —— 目前最快的 macOS 原生终端之一
- Catppuccin —— 颜值与观感兼得的主题家族
- JetBrains Mono —— 程序员最爱的等宽字体

Enjoy your blazing fast terminal! 

最后更新：2026年3月

