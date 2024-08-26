# PIXEL 2 SHAPE

**PIXEL 2 SHAPE** is a Django-based web application that converts 2D images into 3D models using advanced machine learning and deep learning techniques. The application is designed to be user-friendly, allowing users to easily upload images, confirm conversion, and interact with the generated 3D models.

## Table of Contents

1. [Features](#features)
2. [Tech Stack](#tech-stack)
3. [Project Structure](#project-structure)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Screenshots](#screenshots)
7. [Manual Testing](#manual-testing)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Features

- **Image Upload:** Users can upload 2D images for processing.
- **3D Conversion:** Converts the uploaded images into 3D models.
- **Model Preview:** Users can preview and interact with the generated 3D models.
- **User-Friendly Interface:** Clean and simple design for easy navigation.

## Tech Stack

- **Backend Framework:** Django
- **Frontend:** HTML, CSS, JavaScript
- **Database:** SQLite 
- **Image Processing:** Pillow
- **3D Conversion:** Stable Fsat API(credit based)
- **Version Control:** Git

## Project Structure

```plaintext
pixel2shape/
├── manage.py
├── db.sqlite3
├── pixel2shape/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   ├── asgi.py
│   └── __inti__.py
├── upload/
│   ├── migrations/
│   ├── templates/
│   │   └── upload/
│   │       ├── upload.html
│   │       ├── confirm.html
│   │       ├── 3d.html
│   │       ├── upload_success.html
│   │       └── result.html
│   ├── servicess/
│   │   ├── __init__.py
│   │   ├── converter.py
│   │   └── model.py
│   ├── static/
│   ├── views.py
│   ├── models.py
│   ├── urls.py
│   ├── apps.py
│   ├── admin.py
│   ├── tests.py
│   ├── forms.py
│   └── ...
└── media/
    ├── models/
    └── uploads/
venv/
├── Include
├── Lib
├── Scripts
```

## Installation

### Prerequisites

Python 3.x
Django
Pillow

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/varun-jasti/Image3d.git
   cd pixel2shape
   ```

2. **Create and activate a virtual environment:**

   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations:**

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Run the server:**

   ```bash
   python manage.py runserver
   ```

6. **Access the application:**
   - Open your browser and go to `http://127.0.0.1:8000/`.

## Usage

1. **Upload an Image:**
   - Go to the upload page and choose a 2D image to upload.
  
2. **Confirm Conversion:**
   - Review the uploaded image and click the "Convert to 3D" button.

3. **View 3D Model:**
   - Once the conversion is complete, view and interact with the 3D model.

## Screenshots

### Image Upload Page
![Upload Page](Sample%20Demo/Upload%20Page.png)

### Confirmation Page
![Confirmation Page](Sample%20Demo/Confirmation%20Page.png)

### 3D Model Preview
![3D Model](Sample%20Demo/3D%20Model.png)

## Manual Testing

### Test Cases

1. **Image Upload:**
   - **Input:** Valid image file (e.g., .jpg, .png).
   - **Expected Output:** Image is uploaded and stored successfully.

2. **Conversion Confirmation:**
   - **Input:** Confirmation of the uploaded image.
   - **Expected Output:** Image is converted to a 3D model.

3. **3D Model Rendering:**
   - **Input:** View the generated 3D model.
   - **Expected Output:** The model is displayed correctly and is interactive.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

- **Author:** [Varun Kumar Jasti](https://github.com/varun-jasti)
- **Email:** varunkumarjasti@gmail.com
- **LinkedIn:** Viswanadh Varun Kumar Jasti([https://www.linkedin.com/in/yourprofile](https://www.linkedin.com/in/viswanadh-varun-kumar-jasti/)
