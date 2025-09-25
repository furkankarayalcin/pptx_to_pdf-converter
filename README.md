# pptx_to_pdf-converter
GUI tool to convert multiple PPTX files to PDF and merge them in the selected order. Built with Python, Tkinter, and LibreOffice.


PPTX to PDF Converter & Merger
A simple Python GUI application that converts selected PowerPoint (.pptx) files to PDF and merges them into a single PDF. The merge order follows the order in which files are selected.

Features

Convert multiple .pptx files to PDF in batch.
Merge all converted PDFs into a single PDF.
Maintain merge order according to user selection.
Simple GUI interface using Tkinter.
Runs without opening a console window (when packaged as an exe).
Uses LibreOffice for conversion, so no need for Microsoft PowerPoint.

Requirements

Python 3.10+
LibreOffice is installed
Python packages: PyPDF2,tkinter (usually comes with Python)
Install Python packages with:  "pip install PyPDF2"

Usage

Run the Python script: "python pptx_to_pdf_gui.py"
Click "Convert & Merge".
Select the .pptx files you want to convert.
Choose an output folder for PDFs.
Wait until the conversion and merge are done. A pop-up will notify you when finished.

Optional: Build as an EXE

You can package this application as a standalone exe using PyInstaller:
pyinstaller --onefile --noconsole pptx_to_pdf_gui.py
After building, you’ll find the pptx_to_pdf_gui.exe in the dist folder. Run it directly without a console window.

Notes

The merge order follows the order in which you select the PPTX files.
Make sure LibreOffice is installed and the path is correctly set in the script:
libreoffice_path = r"C:\Program Files\LibreOffice\program\soffice.exe"
Works on Windows (tested on Windows 10/11).

License

MIT License – feel free to use and modify!
