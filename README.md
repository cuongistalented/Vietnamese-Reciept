# Receipt Information Extraction (RIE)

### Run the program

REMEMBER: This project is kinda old, so use python around 3.10.11

1. Clone the repo

```
git clone https://github.com/duongttr/vireceipt-information-extraction.git
cd vireceipt-information-extraction
```

2. Install dependency

```
pip install -r requirements.txt
```

3. Run localhost

```
python -m streamlit run VIE_run.py

```

### Fine-tuning model

Download dataset and place it to folder `dataset`, follow this structure:

- `images`: Folder contains receipt images
- `train.json`: Train annotation
- `val.json`: Val annotation

Then run this command:

```python
python train.py --output_dir <output_dir> \
                 --max_steps 15000 \
                 --batch_size 4
```

Check the source code for more parameters.

## References

- Tesseract documentation. Tesseract OCR. (n.d.). Retrieved March 31, 2023, from https://tesseract-ocr.github.io/
- A new state-of-the-art computer vision model. YOLOv8. (n.d.). Retrieved March 31, 2023, from https://yolov8.com/
  Tesseract documentation. Tesseract OCR. (n.d.). Retrieved March 31, 2023, from https://tesseract-ocr.github.io/
- Huang, Y., Lv, T., Cui, L., Lu, Y., & Wei, F. (2022). LayoutLMv3: Pre-training for Document AI with Unified Text and Image Masking. ArXiv. /abs/2204.08387
