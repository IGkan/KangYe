# 康业全景图空间标注与可视化管理系统 (Panorama Management System)

一个基于 WebGL 和 Canvas 开发的轻量级、高性能全景图布点与管理工具。支持 2D 平面图交互标注与 3D 沉浸式全景预览。

## 🚀 项目演示 (Demo)
*https://igkan.github.io/KangYe/*

![image-20260116162237384](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20260116162237384.png)




## ✨ 核心功能
- **多楼层平面图管理**：动态上传、切换平面图，支持画布缩放与平移适配。
- **空间点位标注**：精准的 2D 坐标标注系统，支持点位编号修改与状态实时反馈。
- **3D 沉浸式全景交互**：基于 **Three.js** 的全景查看器，支持多图关联与平滑切换。
- **离线化持久存储**：集成 **IndexedDB** 方案，支持大容量 Base64 全景数据本地存储，刷新不丢失。
- **标准化数据导出**：一键导出 JSON 配置文件，文件名自动包含时间戳及楼层统计。

## 🛠️ 技术栈
- **渲染层**：Three.js (3D), Canvas API (2D)
- **存储层**：IndexedDB (原生浏览器数据库)
- **交互层**：OrbitControls, HTML5 Drag & Drop
- **样式层**：CSS3 Glassmorphism (毛玻璃效果)

## 📦 快速开始
1. 克隆仓库：
   ```bash
   git clone [https://github.com/你的用户名/仓库名.git](https://github.com/你的用户名/仓库名.git)

2. 本地运行
直接双击 index.html 即可运行。
建议通过 VS Code 的 Live Server 插件运行以获得最佳性能。

3. 操作流程

添加楼层: 上传当前层平面图。
点位标注: 切换至“添加点位”模式在图上点击。
关联资源: 选中点位并批量上传全景图。
数据备份: 点击“导出文件”获取标准化命名的 JSON 备份。