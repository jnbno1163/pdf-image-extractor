---
name: pdf-image-extractor
description: Extract images from PDF files with three modes: original (保持原始高清), standard (800x800正方形网站用), compress (50KB内社交分享). Use when user needs to extract product images from furniture catalogs, marketing materials, or any PDF document. Triggers: "提取PDF图片", "PDF转图片", "从PDF导出图片", "extract images from PDF".
---

# PDF图片提取器

从PDF文件中提取图片，支持三种模式。

## 三种模式

| 模式 | 命令 | 用途 |
|------|------|------|
| 原始高清 | `python scripts/extract_original.py` | 印刷、高质量用途 |
| 标准尺寸 | `python scripts/extract_standard.py` | 网站产品图、电商 |
| 压缩优化 | `python scripts/extract_compress.py` | 微信、抖音、小红书 |

## 快速开始

### 1. 安装依赖

```bash
pip install pymupdf pillow
```

### 2. 修改配置

在脚本顶部 `======== 配置区域 ========` 修改：
- `pdf_folder` - PDF文件夹路径
- `output_folder` - 输出路径

### 3. 运行

```bash
# 选择模式
python scripts/extract_original.py    # 原始高清
python scripts/extract_standard.py    # 800x800正方形
python scripts/extract_compress.py    # 压缩分享
```

## 详细说明

- **原始高清模式**: 保持PDF原始分辨率，适合印刷
- **标准尺寸模式**: 800x800正方形，白色背景居中
- **压缩优化模式**: 最大边400px，文件50KB以内

详细参数说明见 `references/config.md`

## 输出结构

```
输出文件夹/
├── PDF文件1/
│   ├── page001_img01.jpg
│   └── ...
└── PDF文件2/
    └── ...
```
