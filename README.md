# PDF Processing Tool

This repository contains a Python script for processing and extracting specific sections from PDF files based on their orientation (landscape or portrait). The tool is designed to loop through nested folders, process PDFs with only one page, and save the extracted regions as new PDF files.

## Features
- Automatically detects if a PDF is in landscape or portrait mode.
- Extracts the bottom-right quadrant for landscape PDFs.
- Extracts the bottom half for portrait PDFs.
- Processes multiple PDFs in nested folders.
- Saves the extracted regions as new PDFs in a specified output folder.

## Requirements
- Python 3.x
- `PyMuPDF` (fitz)
- `PyPDF2`
- `Pillow`

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/PDF-Processing-Tool.git
    ```
2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Define the root folder containing all the PDFs and the output folder in the script.
2. Run the script:
    ```bash
    python process_pdfs.py
    ```

## Example
```python
root_folder = '/path/to/your/pdf/folder'
output_folder = '/path/to/save/extracted/pdfs'

process_pdfs_in_folders(root_folder, output_folder)
