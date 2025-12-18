
# Novo — Desktop Document Generator

Novo is a cross-platform **desktop document generation application** built using **Electron and React**.  
It allows users to generate documents from `.docx` templates by dynamically filling placeholders and exporting the final output as **DOCX or PDF**.

The application is designed to simplify repetitive document creation workflows such as contracts, letters, certificates, and reports.

---

## Features

- Upload `.docx` template files
- Automatically extract placeholders enclosed in `{}`
- Dynamic form generation based on detected placeholders
- Generate completed documents in **DOCX** or **PDF**
- Clean and intuitive desktop UI
- Cross-platform desktop support

---

## Tech Stack

**Frontend**
- React
- JavaScript
- HTML, CSS

**Desktop & Backend**
- Electron
- Node.js
- IPC (Inter-Process Communication)

**Document Processing**
- `docxtemplater`
- `pizzip`
- `libreoffice-convert`

---

## Application Workflow

1. Select a `.docx` template file
2. Placeholders are extracted from the document
3. Input fields are generated automatically
4. Fill in required values
5. Export the document as DOCX or PDF

---

## Project Structure

```
Novo-app/
│
├── public/
│   ├── electron.js
│   ├── preload.js
│   └── index.html
│
├── src/
│   ├── App.js
│   ├── App.css
│   └── index.js
│
├── package.json
└── README.md
```

---

## Installation Guide (Windows)

### Step 1: Install LibreOffice
Download and install **LibreOffice** from the official website or the provided installation link.  
Proceed with default installation settings.

LibreOffice is required for converting DOCX files to PDF.

---

### Step 2: Install Novo (Contract Generator)
Download the Novo application setup file and follow the standard Windows installation steps.

---

### Step 3: Run the Application
When Windows Defender SmartScreen appears:
1. Click **More info**
2. Click **Run anyway**

This is expected for unsigned desktop applications.

---

### Step 4: Prepare Your Template
Ensure all placeholder variables in the `.docx` template are enclosed in **curly braces**.

**Example:**
```
{Name}
{Date}
{Company}
```

---

## Development Setup (For Developers)

### Prerequisites
- Node.js (v18+ recommended)
- npm
- LibreOffice

### Install Dependencies
```bash
npm install
```

### Run in Development Mode
```bash
npm start
```

This launches both the React frontend and Electron desktop window.

---

## Use Cases

- Contract generation
- Offer letters
- Certificates
- Academic and administrative documents
- Repetitive document workflows

---

## Authors

- Parth Malhotra  
- Team Novo

---

## License

MIT License
