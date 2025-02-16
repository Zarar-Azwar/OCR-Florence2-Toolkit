# OCR-Florence2-Toolkit

## 📝 Automatic OCR Annotation Tool

OCR-Florence2-Toolkit is an advanced Optical Character Recognition (OCR) annotation tool leveraging Florence-2. This toolkit enables accurate text extraction from images and supports annotation with bounding box regions. It is designed for AI-driven document processing, automated labeling, and dataset creation.

## 🚀 Features
- Extracts text from images with high accuracy.
- Supports both plain text OCR and OCR with bounding boxes.
- Generates multiple annotation formats: JSON, YOLO, CSV, and human-readable text.
- Easily integrates into AI training pipelines.

## 📦 Installation
Ensure you have the necessary dependencies installed:
```bash
pip install torch transformers pillow numpy opencv-python
```

## 📌 Usage

### 1️⃣ Run OCR on an Image
```python
result = run_example('<OCR>', image)
print(result)
```

### 2️⃣ Run OCR with Region Annotations
```python
result = run_example('<OCR_WITH_REGION>', image)
save_ocr_regions(result)
```

### 3️⃣ Launch OCR Annotation Tool
```python
run_ocr()
```
The tool will prompt you to select either plain OCR or OCR with regions.

## 📂 Output Formats
- **JSON**: Structured text data with bounding box information.
- **YOLO**: Normalized coordinates for object detection models.
- **CSV**: Easy-to-read spreadsheet format.
- **Human-readable text**: Formatted results for quick review.

## 🎯 Example Output (JSON)
```json
{
  "regions": [
    {
      "coordinates": [34, 56, 120, 56, 120, 98, 34, 98],
      "text": "Invoice No: 12345",
      "bbox": { "x1": 34, "y1": 56, "x2": 120, "y2": 98 }
    }
  ]
}
```

## 📖 Future Enhancements
- ✨ Support for additional OCR models.
- 🖼️ Enhanced visualization of OCR annotations.
- 📊 Integration with active learning frameworks.

## 💡 Contribute
Feel free to fork, modify, and contribute! Open issues and PRs are welcome.



