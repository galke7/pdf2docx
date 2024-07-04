
# PDF to DOCX Converter

This project provides a GUI-based tool to convert PDF files to DOCX format. The application uses Python and several libraries to achieve this functionality. The graphical user interface (GUI) is built using Tkinter.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Explanation](#explanation)
- [License](#license)

## Features

- Convert PDF files to DOCX format.
- Supports both text-based and image-based PDFs.
- OCR (Optical Character Recognition) for image-based PDFs.
- Simple and intuitive GUI.

## Requirements

- Python 3.6 or higher
- The following Python libraries:
  - opencv-python-headless
  - pytesseract
  - tkinter
  - pillow
  - pdf2image
  - langchain_community
  - langchain_core
  - numpy

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/pdf2docx.git
   cd pdf2docx
   ```

2. Set up a virtual environment:
   ```sh
   python -m venv myenv
   ```

3. Activate the virtual environment:
   - **Windows**:
     ```sh
     myenv\\Scripts\\activate
     ```
   - **macOS/Linux**:
     ```sh
     source myenv/bin/activate
     ```

4. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```

## Usage

1. Run the application:
   ```sh
   python gui_pdf2dox.py
   ```

2. Use the GUI to select a PDF file and specify the output DOCX file location.

3. Click "Start converting" to convert the PDF to DOCX.

## Explanation

### Imports

- **os**: Provides functions to interact with the operating system.
- **cv2**: OpenCV library for image processing.
- **docx**: Python library for creating and updating Microsoft Word (.docx) files.
- **pytesseract**: Optical Character Recognition (OCR) tool for Python.
- **tkinter**: Standard GUI (Graphical User Interface) package for Python.
- **filedialog** and **messagebox**: Components of tkinter for file dialogs and message boxes.
- **PIL**: Python Imaging Library, for image processing.
- **pdf2image**: Converts PDF files to images.
- **langchain_community** and **langchain_core**: Libraries for handling PDF documents.
- **numpy**: Fundamental package for scientific computing in Python.

### Functions

- **ocr_pdf_with_preprocessing(pdf_path)**: Performs OCR on image-based PDFs with pre-processing steps.
- **select_pdf_file()**: Opens a file dialog to select a PDF file.
- **select_output_location()**: Opens a file dialog to choose the save location for the output file.
- **convert_pdf_to_docx()**: Main function to convert the selected PDF file to a DOCX file.
- **create_gui()**: Sets up and runs the Tkinter GUI.

## License

This project is licensed under the                     GNU GENERAL PUBLIC LICENSE V3. See the [LICENSE](LICENSE) file for more details.
