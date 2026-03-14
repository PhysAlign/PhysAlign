# PhysAlign 项目页面部署清单

## ✅ 已完成的工作

### 1. 核心内容更新
- [x] 论文标题：PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment
- [x] 作者信息（6位作者）及其机构标注
- [x] 完整摘要（从论文提取）
- [x] 动机部分（物理定律和3D感知保真度）
- [x] 方法概述（pipeline图及说明）
- [x] BibTeX引用

### 2. 元数据和SEO
- [x] Primary meta tags (title, description, keywords, author)
- [x] Open Graph tags (Facebook分享预览)
- [x] Twitter Card tags (Twitter分享预览)
- [x] Academic citation metadata (Google Scholar索引)
- [x] Structured data (Schema.org JSON-LD)

### 3. 内容部分
- [x] 标题和作者区域
- [x] 论文链接（Paper, Supplementary, Code, arXiv）
- [x] Teaser视频说明
- [x] Abstract完整内容
- [x] Motivation部分
- [x] Method Overview (含pipeline.png图表)
- [x] Qualitative Results轮播（含4个图表说明）
- [x] Video Comparisons部分
- [x] Example Results视频轮播（3个视频）
- [x] Key Features列表（5个要点）
- [x] Interactive Video Comparisons按钮
- [x] BibTeX引用区

### 4. 相关工作
- [x] PhysGen (arXiv 2024)
- [x] VideoREPA (arXiv 2025)
- [x] ProPhy (arXiv 2024)

### 5. 文件管理
- [x] 复制主论文PDF到 `static/pdfs/PhysAlign.pdf`
- [x] 复制补充材料到 `static/pdfs/supplementary_material.pdf`
- [x] 确认pipeline.png在 `static/images/`目录

## 🔄 需要您完成的最后步骤

### 高优先级（必须完成）

1. **更新arXiv链接**
   - 文件位置：`index.html` 第300行和第60行
   - 查找：`https://arxiv.org/abs/XXXX.XXXXX`
   - 替换为：您的实际arXiv ID（例如：`https://arxiv.org/abs/2501.12345`）

2. **更新GitHub仓库链接**
   - 文件位置：`index.html` 第289行
   - 查找：`https://github.com/YOUR_REPO_HERE`
   - 替换为：您的GitHub仓库URL

3. **更新作者个人主页链接**
   - 文件位置：`index.html` 第248-253行
   - 将所有`https://YOUR_DOMAIN.com`替换为实际的个人主页链接
   - 建议：如果暂时没有个人主页，可以链接到Google Scholar或机构页面

4. **更新网站域名**
   - 全局搜索并替换：`YOUR_DOMAIN.com`
   - 替换为：您的实际域名（例如：`physalign.github.io`或您的自定义域名）

### 中优先级（建议完成）

5. **创建社交媒体预览图**
   - 尺寸：1200x630px
   - 保存为：`static/images/social_preview.png`
   - 用途：在社交媒体分享时显示
   - 当前使用：pipeline.png作为临时预览图

6. **更新Favicon**
   - 当前：使用模板默认图标
   - 建议：创建项目专属图标
   - 位置：`static/images/favicon.ico`

7. **验证所有媒体文件**
   - 检查 `static/videos/banner_video.mp4` 是否为实际的演示视频
   - 检查 `static/videos/carousel1-3.mp4` 是否为正确的示例视频
   - 检查 `static/images/carousel1-4.jpg` 是否为论文中的实际图表

### 低优先级（可选）

8. **添加Twitter handles**
   - 更新作者的Twitter账号（如果有）
   - 当前：使用@WashU作为占位符

9. **压缩媒体文件**
   - 使用TinyPNG压缩图片
   - 使用H.264编码压缩视频
   - 目的：提高页面加载速度

10. **添加Google Analytics或Statcounter**
    - 位置：`index.html` 第513-517行
    - 用途：跟踪页面访问量

## 📝 快速替换命令

### 方法1：使用sed命令（macOS/Linux）

```bash
# 进入项目目录
cd "/Users/zhexioxiong/Library/CloudStorage/GoogleDrive-stevenxiong9325@gmail.com/My Drive/PhysAlign/PhysAlign"

# 替换arXiv ID（假设是2501.12345）
sed -i '' 's/XXXX.XXXXX/2501.12345/g' index.html

# 替换GitHub链接
sed -i '' 's|https://github.com/YOUR_REPO_HERE|https://github.com/yourusername/PhysAlign|g' index.html

# 替换域名
sed -i '' 's/YOUR_DOMAIN.com/physalign.github.io/g' index.html
```

### 方法2：在Cursor中手动编辑

1. 打开 `index.html`
2. 使用 Cmd+F (macOS) 或 Ctrl+F (Windows) 搜索
3. 逐个替换以下内容：
   - `XXXX.XXXXX`
   - `YOUR_REPO_HERE`
   - `YOUR_DOMAIN.com`

## 🌐 本地预览

已启动HTTP服务器，访问：
```
http://localhost:8000/index.html
```

如需重启服务器：
```bash
cd "/Users/zhexioxiong/Library/CloudStorage/GoogleDrive-stevenxiong9325@gmail.com/My Drive/PhysAlign/PhysAlign"
python3 -m http.server 8000
```

## 🚀 部署到GitHub Pages

### 步骤1：创建GitHub仓库
```bash
cd "/Users/zhexioxiong/Library/CloudStorage/GoogleDrive-stevenxiong9325@gmail.com/My Drive/PhysAlign/PhysAlign"
git init
git add .
git commit -m "Initial commit: PhysAlign project page"
git branch -M main
git remote add origin https://github.com/yourusername/PhysAlign.git
git push -u origin main
```

### 步骤2：启用GitHub Pages
1. 进入GitHub仓库设置
2. 找到"Pages"选项
3. Source选择"main"分支
4. 保存后等待几分钟
5. 访问 `https://yourusername.github.io/PhysAlign/`

## 📊 页面结构总览

```
PhysAlign Project Page
├── Hero Section
│   ├── Title
│   ├── Authors (with affiliations)
│   └── Links (Paper, Supp, Code, arXiv)
├── Teaser Video
├── Abstract
├── Motivation
│   ├── General physical laws
│   └── 3D perceptual fidelity
├── Method Overview
│   └── Pipeline diagram (Figure 2)
├── Qualitative Results
│   ├── Bounce scenario
│   ├── Roll scenario
│   ├── Synthetic data (Figure 3)
│   └── WISA test (Figure 4)
├── Video Comparisons
│   └── Link to video_visualization.html
├── Example Results (Video Carousel)
│   ├── Bounce video
│   ├── Roll video
│   └── Complex motion video
├── Key Features
│   └── 5 bullet points
├── Interactive Comparisons Button
├── BibTeX Citation
└── Footer

Additional Features:
├── More Works Dropdown (3 related papers)
├── Scroll to Top Button
└── Copy BibTeX Button
```

## 🎯 质量检查清单

在发布前，请确认：
- [ ] 所有链接可点击且指向正确位置
- [ ] 所有图片正确显示
- [ ] 所有视频可以播放
- [ ] 移动端显示正常（使用浏览器开发者工具测试）
- [ ] BibTeX复制功能正常工作
- [ ] 滚动到顶部按钮功能正常
- [ ] More Works下拉菜单可以展开/收起
- [ ] 所有轮播图可以正常切换
- [ ] 文字无拼写错误
- [ ] 链接在新标签页打开（target="_blank"）

## 📧 联系信息

如需技术支持或有问题，请：
1. 查看 [Academic Project Page Template文档](https://github.com/eliahuhorwitz/Academic-project-page-template)
2. 查看 [Bulma CSS框架文档](https://bulma.io/documentation/)
3. 参考示例网站：https://horwitz.ai/probex

## 🎉 恭喜！

您的PhysAlign项目页面已经准备就绪！完成上述检查清单后即可发布。
