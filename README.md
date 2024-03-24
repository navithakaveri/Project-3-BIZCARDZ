# Project-3-BIZCARDZ
BizCardX: Extracting Business Card Data with OCR

SQL Connection: 
It establishes a connection to a MySQL database using PyMySQL.

home() Function: 
Defines a function home() to display information about the "Biz Card" initiative.

main() Function:
Defines a function main() that currently only sets the title for image text extraction.

Navigation Menu:

Uses the option_menu from a custom module to create a navigation menu with options for "HOME", "UPLOAD", and "DELETE".

Page Handling: Depending on the selected page (page1), it displays different content. If "HOME" is selected, it calls the home() function to display information. If "DELETE" is selected, it provides functionality to delete entries from the database.

extracted_text() Function: Defines a function to extract structured information from OCR results obtained from images. This function seems to parse the OCR results to identify fields like name, designation, company name, contact details, email, website, address, and pincode.

Image Upload and Processing: If the "UPLOAD" option is selected, it allows users to upload an image. Upon upload, it performs OCR using EasyOCR, extracts text, and displays the extracted information in a Pandas DataFrame.

Preview and Upload Modifications: Users can preview and modify the extracted text before uploading it to the database. Once modifications are done, users can click on the "Upload" button to insert the data into the MySQL database.

Database Interaction: It creates a table in the database to store business card information if it doesn't exist already. It inserts the extracted information into the database table.

Success Message: After successful upload to the database, it displays a success message.

Overall, this script combines Streamlit for building a user interface, EasyOCR for text extraction from images, and MySQL for database management to create a simple application for managing business card information
