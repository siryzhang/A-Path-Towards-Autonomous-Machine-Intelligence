# AMI Explorer — LeCun 论文交互式解读

![Cover](cover.png)

## A Path Towards Autonomous Machine Intelligence

对 Yann LeCun 2022 年立场论文的深度交互式可视化解读，涵盖世界模型、JEPA 架构、能量模型与分层规划的完整技术框架。

### ✨ 交互功能

- **六模块认知架构图** — 点击模块查看详细描述与连接关系
- **JEPA vs 生成式 vs 对比学习** — 三种范式的可视化对比切换
- **分层 JEPA（H-JEPA）** — 悬停查看不同时间尺度的预测层级
- **能量地形图** — 可拖动球体直观感受「推理 = 能量最小化」
- **训练范式蛋糕类比** / **JEPA 落地时间线** / **三大路线之争**

### 🚀 在线访问

部署到 GitHub Pages 后，访问：

```
https://<your-username>.github.io/ami-explorer/
```

### 📦 本地运行

这是一个纯静态单文件网页，无需构建：

```bash
# 直接在浏览器中打开
open index.html

# 或者用任意 HTTP 服务器
npx serve .
```

### 🔗 原论文

- **PDF**: [openreview.net/pdf?id=BZ5a1r-kVsf](https://openreview.net/pdf?id=BZ5a1r-kVsf)
- **讨论页**: [openreview.net/forum?id=BZ5a1r-kVsf](https://openreview.net/forum?id=BZ5a1r-kVsf)

### 部署到 GitHub Pages

1. 在 GitHub 上创建新仓库（例如 `ami-explorer`）
2. 将本文件夹内容推送到仓库
3. 进入 Settings → Pages → Source 选择 `main` 分支 → Save
4. 等待几分钟后即可通过上述链接访问

```bash
git init
git add .
git commit -m "AMI Explorer - LeCun 2022 论文交互式解读"
git branch -M main
git remote add origin https://github.com/<your-username>/ami-explorer.git
git push -u origin main
```

### 技术栈

- React 18 (CDN)
- Babel Standalone (浏览器端 JSX 编译)
- Canvas API (神经网络背景动画)
- SVG (架构图 / 能量地形)
- Google Fonts (Playfair Display + DM Sans + Noto Sans SC)

### 📄 License

MIT
