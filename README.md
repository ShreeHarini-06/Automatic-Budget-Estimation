Automated PDF Data Processing and Email Integration - 
            This project automates the extraction and processing of data from PDF files, storing the extracted data into a MongoDB database, and generating reports in PDF and Excel formats. Additionally, it integrates with email services to handle attachment downloads and sends reports via email.
PDF Processing:
      Text Extraction - Extracts specific information such as style number, brand, sizes, commodity, and care address from the first page of a PDF using regular expressions.
      Image Extraction - Extracts the first image from a specified page in the PDF and saves it as a separate image file.
      Table Extraction - Extracts tabular data from the last page of a PDF using pdfplumber for further processing.
Data Management
        MongoDB Storage -  Stores extracted table data into a MongoDB database, including fields such as description, quantity, per rate, and composition.
Report Generation
        Custom PDF Report - Generates a comprehensive PDF report using FPDF that includes extracted text, tables, images, and calculated totals.
        Excel Sheet Generation - Creates an Excel spreadsheet with formatted tabular data using openpyxl.
Email Integration
        Email Sending -  Sends the generated reports as attachments via email using SMTP.
        Attachment Download - Checks for unseen emails in the inbox, downloads PDF attachments, and processes them automatically.
