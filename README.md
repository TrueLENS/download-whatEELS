# WhatEELS

A simple Flask web app to provide downloads for the WhatEELS project.

## Features
- Modern, responsive download page
- Download links for Windows (and other OS in the future)
- Social media meta tags for rich sharing
- Git LFS support for large files

## Requirements
- Python 3.7+
- Flask

## Setup
1. Clone the repository:
   ```
   git clone https://github.com/AndryAlexis/download-whatEELS.git
   cd download-whatEELS
   ```
2. (Recommended) Create and activate a virtual environment:
   ```
   python -m venv .venv
   .venv\Scripts\activate  # On Windows
   source .venv/bin/activate  # On Mac/Linux
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. (Optional) Set up Git LFS for large files:
   ```
   git lfs install
   git lfs track "downloads/*.zip"
   git add .gitattributes
   git commit -m "Track zip files with Git LFS"
   ```

## Usage
1. Place your downloadable files (e.g., WhatEELS.zip) in the `downloads/` folder.
2. Run the Flask app:
   ```
   python app.py
   ```
3. Open your browser and go to [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

## Deployment
- For static sites, use GitHub Pages (HTML/CSS/JS only, no Flask backend).
- For Flask backend, deploy to Render, Heroku, PythonAnywhere, or similar.

## License
MIT
