# 世界地震监测 - Web GIS 课程作业 (2.5)

## 📋 作业要求

选择案例：**展示世界各地最近的地震情况**

### 基本要求
1. ✅ **配置适当的图层样式** — 按震级大小使用不同颜色和尺寸的圆形标记
2. ✅ **配置适当的弹出窗口** — 包含震级、深度、时间、海啸预警等详细信息
3. ✅ **将 Web 地图转化为 Web 应用程序** — Leaflet + 高德底图的完整交互式应用
4. ✅ **分享所创建的 Web 地图和应用程序** — 可部署到 GitHub Pages

### 数据来源
- 本地模拟数据，涵盖全球主要地震带（中国及周边、环太平洋、欧亚、美洲等）
- 共 26 个地震点，震级范围 2.5~8.4 级

## 📁 文件结构

```
第三个作业/
├── index.html              # 主应用页面 (HTML + CSS + JavaScript)
├── earthquake_data.csv     # 地震数据文件 (CSV格式)
└── README.md               # 本说明文件
```

## 🚀 部署到 GitHub Pages（获取提交URL）

### 第一步：创建 GitHub 仓库

1. 打开 [GitHub.com](https://github.com) 并登录
2. 点击 **New repository**（新建仓库）
3. 仓库名随意，如 `webgis-earthquake`
4. 设置为 **Public**（公开）
5. 点击 **Create repository**

### 第二步：上传文件

```bash
git init
git add .
git commit -m "提交地震监测应用"
git remote add origin https://github.com/你的用户名/webgis-earthquake.git
git branch -M main
git push -u origin main
```

或直接在 GitHub 网页上传 `第三个作业` 目录下的所有文件。

### 第三步：开启 GitHub Pages

1. 仓库 → **Settings** → **Pages**
2. **Branch** 选 `main`，**文件夹** 选 `/root`
3. 点击 **Save**
4. 等待 1-2 分钟，获得 URL

## 📄 提交内容填写

| 提交项 | 填写内容 |
|--------|---------|
| **(1) 要素图层的服务URL** | `数据以GeoJSON格式嵌入应用，部署后应用内数据即为要素服务` |
| **(2) Web地图的URL** | `https://你的用户名.github.io/webgis-earthquake/index.html` |
| **(3) Web应用程序的URL** | `https://你的用户名.github.io/webgis-earthquake/index.html` |

## 🎯 功能特性

- 🌍 **世界地图展示** — Leaflet + 高德地图底图
- 🔴 **震级样式渲染** — 按震级使用不同颜色和尺寸圆圈标记
- 📊 **震级分布图表** — 纯 Canvas 绘制的柱状图（零外部依赖）
- 📋 **地震列表** — 按时间排序，点击跳转到地图位置
- 🔍 **数据筛选** — 按最小震级筛选
- 📍 **弹出窗口** — 震级、深度、时间等详细信息
- 📱 **响应式设计** — 完美适配手机和电脑
- 🎨 **暗色主题** — 专业的深色 UI 设计

## 🛠️ 技术栈

- [Leaflet](https://leafletjs.com/) + 高德地图底图 — 轻量级地图引擎
- Canvas API — 图表绘制（零外部依赖）
- 纯 HTML/CSS/JavaScript — 无需任何框架
