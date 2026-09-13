# PiliPlus SideStore / AltStore 订阅源

[![Sync PiliPlus Source](https://github.com/JiPengLin/piliplus-sidestore-source/actions/workflows/sync.yml/badge.svg)](https://github.com/JiPengLin/piliplus-sidestore-source/actions/workflows/sync.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

专为 **SideStore** 与 **LiveContainer** 适配的非官方 [PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus) 自动更新源。

---

## 快速添加订阅

### 方式一：一键唤起添加（推荐）

在 iOS 设备上使用 Safari 浏览器点击下方按钮，可直接呼起 SideStore 并添加源：

[![Add to SideStore](https://img.shields.io/badge/Add_Source_to-SideStore-00AEEF?style=for-the-badge&logo=apple)](https://stikstore.app/altdirect/?url=https://JiPengLin.github.io/piliplus-sidestore-source/apps.json)

---

### 方式二：手动复制订阅链接

**推荐链接（GitHub Pages 直链）：**
```text
https://JiPengLin.github.io/piliplus-sidestore-source/apps.json
```

**备用直链（Raw 直链）：**
```text
https://raw.githubusercontent.com/JiPengLin/piliplus-sidestore-source/main/apps.json
```

**添加步骤：**
1. 复制上述链接；
2. 打开 iPhone 上的 **SideStore**；
3. 进入底部的 **Sources** 标签页；
4. 点击右上角 **`+`** 号，粘贴链接并点击 **Add** 保存。

---

## 特性说明

- **全自动同步**：基于 GitHub Actions，每 2 小时定时轮询官方上游 Releases 并自动维护发布清单。
- **原生包名对齐**：精准匹配官方 iOS 包名 `com.example.piliplus`。在 LiveContainer 中覆盖升级不会生成重复应用，不丢失本地数据，不破坏既有的 Launch URL / 快捷方式。
- **规范元数据**：包含应用图标、高清预览轮播截图、更新日志提取及语义化版本精准排序。
- **轻量可靠**：采用 Python 原生标准库生成，配置专属 GitHub Token 鉴权，无第三方依赖污染，无 API 限流风险。

---

## 免责声明与致谢

1. 本项目仅为自动化生成 AltStore / SideStore 规范元数据的索引脚本工具，**不存储、不修改、不分发任何二进制 IPA 文件**。所有应用安装包均直链来源于上游官方仓库 Releases。
2. 原项目版权归 [bggRGjQaUbCoE/PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus) 及原作者所有。
