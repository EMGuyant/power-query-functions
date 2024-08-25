# Power Query Data Transformation Template

## Overview

This repository contains a Power BI template designed to automate the loading, cleaning, and transformation of CSV files stored in SharePoint. The template leverages Power Query functions and parameters to create a flexible and reusable solution for data preparation, ensuring that datasets are consistently cleaned and properly formatted for analysis.

Included in this repository are:
- A set of sample source CSV files.
- A Power BI template file (.pbit) that integrates the parameters, functions, and queries discussed in the accompanying blog post.

## Contents

- **`Sample_CSVs/`**: This directory contains sample CSV files that can be used to test the template's functionality. These files simulate typical data that might be loaded from SharePoint, including examples with various common data issues (e.g., blank rows, inconsistent text formatting, duplicate records).
  
- **`PowerBI_Template.pbit`**: This is the Power BI template file that includes the Power Query parameters, custom functions, and queries necessary to replicate the solution discussed in the blog post. The template is designed to be easily adaptable to different datasets and SharePoint locations.

## Getting Started

### Prerequisites

- **Power BI Desktop**: Ensure that you have the latest version of Power BI Desktop installed.
- **Access to SharePoint**: You should have access to a SharePoint site where your CSV files are stored, as the template is designed to pull data from SharePoint.

### How to Use the Template

1. **Clone the Repository**:
   - Clone or download this repository to your local machine.
   - Ensure you have access to the `Sample_CSVs` directory and the `PowerBI_Template.pbit` file.

2. **Open the Power BI Template**:
   - Open the `PowerBI_Template.pbit` file in Power BI Desktop.

3. **Configure Parameters**:
   - When opening the template, you will be prompted to enter values for several Power Query parameters:
     - **`SharePoint Site Url`**: Enter the URL of your SharePoint site.
     - **`SharePoint Folder Path`**: Specify the path to the folder containing your CSV files.
     - **`textFormatCase`**: Select a text formatting case.
     - **`columnDataTypes`**: Define the data types for each column in your dataset.
     - **`textColumns`**: Provide a comma-separated list of columns that require text transformations.
     - **`replaceValue`**: Specify the value to replace errors in your dataset (if applicable).
     - **`errorHandlingOption`**: Choose how to handle errors (`RemoveErrors` or `ReplaceErrors`).
     - **`viewErrorSummary`**: Decide whether to display a summary of errors (`true` or `false`).

4. **Load and Transform Data**:
   - The template will automatically connect to the specified SharePoint site, load the CSV files, and apply the predefined transformations. The final cleaned dataset will be ready for analysis within Power BI.

5. **Review and Customize**:
   - Review the transformed data in Power BI. You can further customize the template by modifying the Power Query functions or parameters as needed.
