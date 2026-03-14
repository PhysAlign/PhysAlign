# PhysAlign: Physics-Coherent Image-to-Video Generation

Official project page for **PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment**

## 🌐 Project Page

**Live Demo**: [Coming Soon - Will be available at https://yourusername.github.io/PhysAlign/]

**Local Preview**: `http://localhost:8000/index.html`

## 📄 Paper Information

- **Title**: PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment
- **Authors**: Zhexiao Xiong, Yizhi Song, Liu He, Wei Xiong, Yu Yuan, Nathan Jacobs
- **Institutions**: Washington University in St. Louis, Purdue University, NVIDIA
- **Year**: 2025
- **Venue**: arXiv preprint

## 🎯 Abstract

Video Diffusion Models (VDMs) are a promising approach for world simulation, which have wide-ranging applications in robotics and media generation. However, current models often produce temporally incoherent content that violates basic physical intuition, significantly limiting their utility. We introduce **PhysAlign**, a novel physics-coherence framework for image-to-video generation that explicitly addresses this limitation through image and 3D representation alignment. Our method improves physical consistency by leveraging a new training pipeline built on a large-scale synthetic dataset equipped with accurate, granular physics and 3D state annotations.

## 🚀 Quick Start

### View Locally

```bash
# Clone or navigate to the repository
cd PhysAlign

# Start a local server
python3 -m http.server 8000

# Open in browser
# http://localhost:8000/index.html
```

### Deploy to GitHub Pages

```bash
# Initialize git repository
git init
git add .
git commit -m "Initial commit: PhysAlign project page"

# Push to GitHub
git branch -M main
git remote add origin https://github.com/yourusername/PhysAlign.git
git push -u origin main

# Enable GitHub Pages in repository settings
# Your site will be live at: https://yourusername.github.io/PhysAlign/
```

## 📁 Repository Structure

```
PhysAlign/
├── index.html                          # Main project page
├── video_visualization.html            # Interactive video comparisons
├── static/
│   ├── css/                           # Stylesheets
│   ├── js/                            # JavaScript files
│   ├── images/
│   │   ├── pipeline.png               # Method pipeline diagram
│   │   └── carousel1-4.jpg            # Result visualizations
│   ├── pdfs/
│   │   ├── PhysAlign.pdf              # Main paper (47MB)
│   │   └── supplementary_material.pdf  # Supplementary material (4MB)
│   └── videos/
│       ├── banner_video.mp4           # Teaser video
│       └── carousel1-3.mp4            # Example videos
├── PROJECT_PAGE_GUIDE.md              # Detailed usage guide (English)
├── DEPLOYMENT_CHECKLIST.md            # Deployment checklist (English)
├── 使用说明.md                         # Usage guide (Chinese)
└── SUMMARY.md                         # Completion summary
```

## ✅ Features

- 📱 **Responsive Design**: Works on all devices (mobile, tablet, desktop)
- 🔍 **SEO Optimized**: Complete meta tags and structured data for search engines
- 🎨 **Modern UI**: Clean, professional academic design
- 🎬 **Rich Media**: Support for videos, images, and interactive carousels
- 📋 **One-Click Copy**: BibTeX citation with copy button
- 🔗 **Social Sharing**: Optimized for Facebook, Twitter, LinkedIn
- 📚 **Related Works**: Dropdown menu for lab's other publications
- 🎯 **Interactive**: Link to detailed video comparison page

## 🔧 Before Publishing

### Required Updates

1. **arXiv ID**: Replace `XXXX.XXXXX` with your actual arXiv ID
2. **GitHub Repository**: Replace `YOUR_REPO_HERE` with your repository name
3. **Domain Name**: Replace `YOUR_DOMAIN.com` with your actual domain
4. **Author Links**: Update personal homepage links for all authors

### Quick Replace Commands

```bash
# Replace arXiv ID (example: 2501.12345)
sed -i '' 's/XXXX.XXXXX/2501.12345/g' index.html

# Replace GitHub repository
sed -i '' 's|YOUR_REPO_HERE|yourusername/PhysAlign|g' index.html

# Replace domain
sed -i '' 's/YOUR_DOMAIN.com/physalign.github.io/g' index.html
```

## 📖 Citation

```bibtex
@article{xiong2025physalign,
  title={PhysAlign: Physics-Coherent Image-to-Video Generation through Feature and 3D Representation Alignment},
  author={Xiong, Zhexiao and Song, Yizhi and He, Liu and Xiong, Wei and Yuan, Yu and Jacobs, Nathan},
  journal={arXiv preprint},
  year={2025}
}
```

## 🔗 Links

- **Paper**: [PDF](static/pdfs/PhysAlign.pdf)
- **Supplementary**: [PDF](static/pdfs/supplementary_material.pdf)
- **Code**: [Coming Soon]
- **arXiv**: [Coming Soon]
- **Interactive Comparisons**: [video_visualization.html](video_visualization.html)

## 🤝 Related Works

- [PhysGen: Rigid-Body Physics-Grounded Image-to-Video Generation](https://arxiv.org/abs/2409.18964) (arXiv 2024)
- [VideoREPA: Learning Physics for Video Generation through Relational Alignment](https://arxiv.org/abs/2505.23656) (arXiv 2025)
- [ProPhy: Progressive Physical Alignment for Dynamic World Simulation](https://arxiv.org/abs/2512.05564) (arXiv 2024)

## 📝 Documentation

- **English Guide**: [PROJECT_PAGE_GUIDE.md](PROJECT_PAGE_GUIDE.md)
- **中文说明**: [使用说明.md](使用说明.md)
- **Deployment**: [DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md)
- **Summary**: [SUMMARY.md](SUMMARY.md)

## 📄 License

This website is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

The template is based on the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template) which was adopted from [Nerfies](https://nerfies.github.io/).

## 🙏 Acknowledgments

This project page was built using:
- [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
- [Bulma CSS Framework](https://bulma.io/)
- [Font Awesome Icons](https://fontawesome.com/)
- [Academicons](https://jpswalsh.github.io/academicons/)

---

**For questions or issues, please refer to the documentation files or open an issue on GitHub.**
