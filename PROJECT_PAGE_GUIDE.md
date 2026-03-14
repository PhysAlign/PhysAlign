# PhysAlign 项目页面使用指南

## 📋 已完成的更新

### 1. 元数据和SEO
- ✅ 更新了页面标题为："PhysAlign: Physics-Coherent Image-to-Video Generation"
- ✅ 添加了所有6位作者的信息
- ✅ 更新了机构信息：Washington University in St. Louis, Purdue University, NVIDIA
- ✅ 设置了适当的关键词：video generation, physics simulation, image-to-video, diffusion models等
- ✅ 配置了Open Graph和Twitter卡片元数据

### 2. 主要内容部分

#### 标题和作者
- 标题：PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment
- 作者：
  - Zhexiao Xiong¹
  - Yizhi Song²
  - Liu He²
  - Wei Xiong³
  - Yu Yuan²
  - Nathan Jacobs¹
- 机构：¹WashU, ²Purdue, ³NVIDIA

#### 摘要
完整的论文摘要，介绍了PhysAlign框架的主要贡献和创新点。

#### 动机部分
解释了当前VDM模型的局限性，以及PhysAlign关注的两个关键维度：
- 通用物理定律
- 3D感知保真度

#### 方法概述
- 显示pipeline.png图表
- 包含详细的图表说明（Figure 2）

#### 定性结果
使用carousel展示4个主要图表：
- Bounce场景比较
- Roll场景比较
- 合成数据可视化（Figure 3）
- WISA测试结果（Figure 4）

#### 示例结果视频
3个视频轮播，展示：
- Bounce场景
- Roll场景
- 复杂运动场景

#### 关键特性
列出5个主要特点：
- 物理一致性生成
- 3D感知保真度
- 合成数据管道
- 统一对齐方法
- SOTA性能

#### 交互式视频比较
- 大按钮链接到video_visualization.html页面
- 用户可以查看与CogVideoX-5B, Hunyuan I2V, Wan2.2的详细对比

#### BibTeX引用
```bibtex
@article{xiong2025physalign,
  title={PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment},
  author={Xiong, Zhexiao and Song, Yizhi and He, Liu and Xiong, Wei and Yuan, Yu and Jacobs, Nathan},
  journal={arXiv preprint},
  year={2025}
}
```

### 3. 相关工作
更新了"More Works"下拉菜单，包含3个相关论文：
- PhysGen (arXiv 2024)
- VideoREPA (arXiv 2025)
- ProPhy (arXiv 2024)

### 4. 文件组织
```
PhysAlign/
├── index.html (主项目页面)
├── video_visualization.html (交互式视频比较页面)
├── static/
│   ├── pdfs/
│   │   ├── PhysAlign.pdf (主论文)
│   │   └── supplementary_material.pdf (补充材料)
│   ├── images/
│   │   ├── pipeline.png (方法流程图)
│   │   ├── carousel1-4.jpg (结果图片)
│   │   └── favicon.ico
│   └── videos/
│       ├── banner_video.mp4 (顶部视频)
│       └── carousel1-3.mp4 (示例视频)
```

## 🔧 下一步需要做的事情

### 必须更新的项目
1. **arXiv链接**: 将`https://arxiv.org/abs/XXXX.XXXXX`替换为实际的arXiv ID
2. **GitHub仓库**: 将`https://github.com/YOUR_REPO_HERE`替换为实际的GitHub链接
3. **作者个人链接**: 更新每位作者的个人主页链接（目前都是YOUR_DOMAIN.com）
4. **域名**: 将所有`YOUR_DOMAIN.com`替换为实际的网站域名

### 可选更新
1. **社交预览图**: 创建1200x630px的社交媒体预览图，保存为`static/images/social_preview.png`
2. **Favicon**: 替换`static/images/favicon.ico`为自定义图标
3. **视频内容**: 确保所有视频文件（banner_video.mp4, carousel1-3.mp4）都是实际的演示视频
4. **图片内容**: 确保carousel1-4.jpg包含论文中的实际图表

## 🚀 如何本地查看

已启动HTTP服务器，访问：
```bash
http://localhost:8000/index.html
```

或者在新终端中运行：
```bash
cd "/path/to/PhysAlign"
python3 -m http.server 8000
```

## 📝 快速替换指令

### 更新arXiv链接
假设您的arXiv ID是2501.12345，运行：
```bash
# 在index.html中替换
sed -i '' 's/XXXX.XXXXX/2501.12345/g' index.html
```

### 更新GitHub链接
```bash
sed -i '' 's|https://github.com/YOUR_REPO_HERE|https://github.com/yourusername/PhysAlign|g' index.html
```

### 更新域名
```bash
sed -i '' 's/YOUR_DOMAIN.com/physalign.github.io/g' index.html
```

## ✨ 特色功能

- **响应式设计**: 自动适应移动设备和桌面
- **SEO优化**: 包含完整的元标签和结构化数据
- **复制BibTeX**: 一键复制引用信息
- **图片轮播**: 自动播放的图片展示
- **视频轮播**: 循环播放的示例视频
- **滚动到顶部按钮**: 便捷的导航
- **相关工作下拉菜单**: 展示实验室的其他研究

## 🎨 自定义提示

1. 所有图片应该压缩优化（使用TinyPNG等工具）
2. 大视频建议上传到YouTube并嵌入
3. 确保所有外部链接在新标签页打开
4. 测试移动端显示效果

## 📞 技术支持

如需进一步自定义，请参考：
- [Bulma CSS框架文档](https://bulma.io/documentation/)
- [原始模板文档](https://github.com/eliahuhorwitz/Academic-project-page-template)
