# Data Repository

## Overview

This repository contains annual financial reports for various companies in both PDF and JSON formats. The JSON files contain the same financial data as the PDFs but structured for ease of use in markdown format. Each folder is named after the company it represents, and within each folder, you'll find the financial reports for the years available.

## Folder Structure

- **ABB**
  - `2021.json`
  - `2021_A.pdf`
  - `2021_B.pdf`
  - `2022.json`
  - `2022.pdf`
  - `2023.json`
  - `2023.pdf`
- **IBM**
- **PostFinance**
- **Raiffeisen**
- **Siemens**
- **UBS**

## JSON Structure

Each JSON file contains structured data for the corresponding financial report. The structure of the `content` field is the most important part as it provides the financial data in markdown format, making it easy to use and integrate:

```json
{
	"status": "succeeded",
	"createdDateTime": "2024-06-21T10:50:30Z",
	"lastUpdatedDateTime": "2024-06-21T10:51:04Z",
	"analyzeResult": {
		"apiVersion": "2023-10-31-preview",
		"modelId": "prebuilt-layout",
		"stringIndexType": "utf16CodeUnit",
		"content": "..."
	}
}
```

- **content**: The actual content of the financial report in markdown format.

## Usage

The PDF files are the original financial reports, which can be viewed using any standard PDF reader. The JSON files provide a structured format of the same reports, making it easy to integrate and use in various applications. The markdown format in the JSON is especially suitable for feeding into OpenAI GPT models for analysis and processing.