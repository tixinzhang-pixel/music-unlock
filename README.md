# 🎵 MusicUnlock · 全平台音乐格式解密与无损转换工具

> **100% 浏览器本地运算 · 零隐私泄露 · 全主流音乐平台兼容 · 开箱即用**

基于 WebAssembly 与现代密码学算法实现的纯前端在线音乐解密工具。无需将文件上传至服务器，直接在浏览器本地内存中秒级完成各类加密音乐文件的解密还原与标签提取。

---

## 🌟 核心特性

- 🔒 **100% 纯前端离线解密**：所有音频数据均在本地运行，零服务器成本，零隐私泄露风险。
- ⚡ **原生 WASM 极速解码**：内嵌 `@xhacker/qmcwasm` 与 `@xhacker/kgmwasm` 编译模块，解密速度可达 20MB/s+。
- 🎶 **全平台主流格式兼容**：
  - **网易云音乐**：`.ncm`（完整提取歌曲名、歌手、专辑与高清嵌入封面）
  - **QQ音乐 / 腾讯音乐**：`.qmc0`, `.qmc2`, `.qmc3`, `.qmc4`, `.qmc6`, `.qmc8`, `.qmcflac`, `.qmcogg`, `.tkm`, `.bkcmp3`, `.bkcflac` 以及新版 `.mflac`, `.mflac0`, `.mgg`, `.mgg0`, `.mgg1`
  - **酷狗音乐**：`.kgm`, `.kgma`, `.vpr`
  - **酷我音乐**：`.kwm`
  - **QQ音乐缓存**：`.tm0`, `.tm2`, `.tm6`
  - **虾米音乐**：`.xm`
- 👑 **云端深度解析专区（双轨制商业化闭环）**：
  - 针对高版本客户端动态加密保护（如 Mac 版 QQ 音乐 `musicex` 等本地缺乏离线密钥的文件），提供云端元数据指纹无损匹配通道。
  - 采用**极简扫码信任制**（支持微信赞赏与支付宝扫码），小额微支付（¥1.99）秒级放行，实现工具的可持续盈利。
- 📦 **批量与便捷操作**：支持多选与拖拽，提供内置轻量播放器即时试听、单曲下载及一键打包 ZIP 批量下载。
- 🎨 **极简纯白设计**：秉持 Notion / Apple 式极简设计风格，视觉清爽高级。

---

## 🚀 部署指南

### 方式一：GitHub Pages 自动部署（已集成）
本仓库已配置 GitHub Actions 自动部署流水线：
1. 仓库默认分支 `main` 每次更新时会自动触发构建并发布至 GitHub Pages。
2. 在仓库设置页面中：**Settings** -> **Pages** -> **Build and deployment** -> **Source** 选择 **GitHub Actions** 即可。

### 方式二：Cloudflare Pages（推荐，全球极速 CDN）
1. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)。
2. 进入 **Workers & Pages** -> **Create application** -> **Pages** -> **Connect to Git**。
3. 选择本仓库 `music-unlock`，构建输出目录留空或填写根目录 `.`，点击 **Save and Deploy** 即可获得全球秒开的专属免费二级域名（如 `https://music-unlock.pages.dev`）。

### 方式三：本地离线运行
直接双击打开 `index.html`，无需安装任何运行环境或依赖，完全支持离线在本地浏览器中运行！

---

## ☕ 赞助支持

如果本项目对您有所帮助，欢迎赞赏支持！

| 微信赞赏 (MOMO 共创中心) | 支付宝 (Momo 音乐) |
| :---: | :---: |
| ![微信支付](assets/wechat_pay.jpg) | ![支付宝](assets/alipay.jpg) |

---

## 📄 免责声明
本工具仅供技术交流与个人合法已购音乐的本地离线备份使用，请勿用于任何商业侵权行为。
