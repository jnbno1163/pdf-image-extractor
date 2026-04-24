PDF Image Extractor

A powerful tool to extract images from PDF files with three output modes for different use cases.

Three Modes

Mode 1: Original Quality
- Keep original PDF image resolution
- Best for: Printing, high-quality output

Mode 2: Standard Size
- Output: 800x800 square images
- Best for: Website product images, e-commerce

Mode 3: Compressed
- Max 400px, under 50KB
- Best for: WeChat, Douyin, social media sharing

Quick Start

# Install dependencies
pip install pymupdf pillow

# Extract images
python scripts/extract_original.py    # Keep original quality
python scripts/extract_standard.py    # Standard 800x800
python scripts/extract_compress.py    # Compressed for sharing

Output Structure

output_folder/
    PDF_Name_1/
        page001_img01.jpg
        ...
    PDF_Name_2/
        ...

Configuration

Edit the CONFIG section at the top of each script:
- pdf_folder - Path to your PDF folder
- output_folder - Where to save extracted images

Requirements

- Python 3.7+
- PyMuPDF (pymupdf)
- Pillow (PIL)

Use Cases

- Furniture manufacturers: Extract catalog images for printing
- E-commerce: Prepare product images for websites
- Sales: Compress images for WeChat Moments, Douyin

License: MIT
Author: xiaojie @ jnbno1
