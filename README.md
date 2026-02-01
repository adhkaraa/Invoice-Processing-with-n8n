# Invoice Data Processing with n8n

## Problem 
Organizations often receive documents invoice in formats like PDF or PNG that contain important information (vendor, date, total amount, etc.). These are usually processed manually, which is time-consuming, error-prone, and not scalable.

## Solution
This pipeline automates the entire process:
1. Detects new documents uploaded to Google Drive
2. Extracts text using OCR (for both PDF and images)
3. Uses an LLM to interpret and structure the information
4. Stores extracted data in Google Sheets
5. Moves processed files to an archive folder

## Workflow n8n
![Workflow](Workflow.png)

