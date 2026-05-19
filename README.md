# 📄 PDF Image Extractor · PDF图片提取器

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![ClawHub](https://img.shields.io/badge/ClawHub-pdf--image--extractor-orange)](https://clawhub.ai)

**从PDF中提取图片，提供三种输出模式。** 专为家具制造商、电商运营、市场营销人员设计，一条命令即可将产品目录PDF转换为可直接使用的图片。

**Extract images from PDF files with three output modes.** Designed for furniture manufacturers, e-commerce operators, and marketers. Convert product catalogs from PDF to ready-to-use images with a single command.

---

## 🎯 三种模式 | Three Modes

| 模式 Mode | 命令 Command | 输出 Output | 适用场景 Best For |
|-----------|-------------|-------------|-------------------|
| **Original** 原图 | `python scripts/extract_original.py` | 原始尺寸/质量 | 印刷、画册、高清存档 |
| **Standard** 标准 | `python scripts/extract_standard.py` | 800×800 方形 JPG | 网站、电商平台、小程序 |
| **Compress** 压缩 | `python scripts/extract_compress.py` | <50KB 压缩图 | 微信朋友圈、抖音、社交媒体 |

---

## ⚡ 快速开始 | Quick Start

```bash
# 1. 安装依赖 | Install dependencies
pip install pymupdf pillow

# 2. 配置路径（编辑每个脚本顶部的 CONFIG 部分）
#    Configure paths (edit CONFIG section at top of each script):
#    - pdf_folder: PDF 文件夹路径
#    - output_folder: 图片输出路径

# 3. 运行 | Run
python scripts/extract_original.py    # 原图 · Original
python scripts/extract_standard.py    # 标准 · Standard
python scripts/extract_compress.py    # 压缩 · Compress
```

---

## 📁 输出结构 | Output Structure

```
output_folder/
├── PDF_Name_1/
│   ├── page001_img01.jpg
│   ├── page001_img02.jpg
│   └── ...
└── PDF_Name_2/
    └── ...
```

每页的图片按顺序编号，按来源PDF独立分文件夹存放。

Images are numbered by page, organized in separate folders per source PDF.

---

## 📋 系统要求 | Requirements

- Python 3.7+
- [PyMuPDF](https://pypi.org/project/PyMuPDF/) (pymupdf)
- [Pillow](https://pypi.org/project/Pillow/) (PIL)

---

## 💡 典型场景 | Use Cases

| 行业 Industry | 场景 Scenario |
|--------------|---------------|
| 🪑 家具制造 Furniture | 将产品画册PDF转为图片，直接用于画册印刷（Original）或发给经销商（Compress） |
| 🛒 电商运营 E-commerce | 供应商发的PDF产品目录 → 800×800标准图片 → 一键上架 |
| 📱 社交媒体 Social Media | PDF素材 → 压缩至50KB以内 → 微信/抖音直接发 |
| 🏢 市场营销 Marketing | 投标材料PDF中的效果图快速提取 |

---

## 🔧 在 OpenClaw 中使用 | Use with OpenClaw

此技能已发布到 ClawHub，OpenClaw 用户可直接安装：

```bash
npx clawhub@latest install pdf-image-extractor
```

触发词：`extract PDF images` / `PDF to images` / `extract from PDF` / `提取PDF图片`

---

## 🤝 贡献 | Contributing

欢迎提 Issue 和 PR！如果你有新的输出格式需求（如 WebP、SVG 等），欢迎贡献代码。

Issues and PRs are welcome! If you need new output formats (WebP, SVG, etc.), feel free to contribute.

---

**Author:** [小杰 @ AI家具链](https://github.com/jnbno1163)  
**License:** MIT  
**ClawHub:** [pdf-image-extractor](https://clawhub.ai)
