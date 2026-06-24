# File Upload API

A simple Flask REST API to upload and list files.

## Features

- Upload files
- View uploaded files
- JSON responses
- Beginner-friendly project

## Project Structure

```
file-upload-api/
│── app.py
│── requirements.txt
│── README.md
│── uploads/
```

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/file-upload-api.git
```

### Navigate to the project

```bash
cd file-upload-api
```

### Install dependencies

```bash
pip install -r requirements.txt
```

## Run the project

```bash
python app.py
```

Server runs at:

```
http://127.0.0.1:5000
```

## API Endpoints

### Home

```
GET /
```

Response

```json
{
  "message": "Welcome to File Upload API"
}
```

---

### Upload File

```
POST /upload
```

Use **Postman**:

- Method: POST
- Body → form-data
- Key: `file`
- Type: File
- Select any file

Response

```json
{
  "message": "File uploaded successfully",
  "filename": "example.pdf"
}
```

---

### List Uploaded Files

```
GET /files
```

Response

```json
[
  "example.pdf",
  "image.png"
]
```

## Technologies Used

- Python
- Flask
- REST API
