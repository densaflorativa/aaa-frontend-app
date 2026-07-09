# Image Text Recognition — Web App

A web application for uploading an image and extracting text from it (OCR), built as part of Avito Analytics Academy (Frontend for DS Engineers module).

## Stack

- **FastAPI** — backend and routing
- **Jinja2** — HTML templating
- **Bootstrap** — styling
- **EasyOCR** — text detection and recognition on uploaded images
- **Pillow (PIL)** — image processing, drawing detected text regions on the image

## How it works

1. User uploads an image through the web interface
2. EasyOCR detects text regions and recognizes the text
3. The app draws bounding boxes around detected text on the image and returns both the annotated image and the extracted text

## Run locally

```bash
python3.12 -m venv venv
source venv/bin/activate
pip install -r requirements.txt -r requirements-dev.txt
make download   # downloads the OCR model
make dev
```

## Tests

```bash
make test
```
