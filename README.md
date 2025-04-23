# Email_Classification_for_support_team

This project is a machine learning-powered solution to **classify incoming support emails** and **mask Personally Identifiable Information (PII)** before further processing. Designed as part of a company internship assignment, this system also includes a fully functional API built using FastAPI and/or Flask, deployable to Hugging Face Spaces or any cloud platform.

---

##  Features

-  Classifies support emails into predefined categories.
-  Applies PII masking using SpaCy and custom regex.
-  REST API endpoints for classification and masking.
-  Pre-trained models with sample training data.
-  Ready for local and cloud deployment.

---

##  Tech Stack

- Python 3.8+
- FastAPI / Flask
- Scikit-learn, Pandas, Transformers
- SpaCy (for NER-based masking)
- Uvicorn (for ASGI serving)

---

##  Project Structure
  Email_Classification_Siddharthan/ │ ├── app.py # Main FastAPI application ├── app_flask.py # Flask version (alternative) ├── api.py # Classification + masking logic ├── Applying_PII_Masking.py # Script for PII    masking ├── email_masked_for_training.csv # Sample masked data ├── README.md # Project documentation ├── LICENSE ├── .gitignore ├── Final_output_API_Endpoints.pdf ├── Report.pdf


---

## 🛠️ Setup and Execution

1. **Install Dependencies**:

bash
pip install -r requirements.txt

Or manually:

bash
Copy
Edit
pip install fastapi uvicorn transformers pandas scikit-learn spacy
python -m spacy download en_core_web_sm
Run API (FastAPI):

bash
Copy
Edit
uvicorn app:app --reload
Visit: http://127.0.0.1:8000/docs

Run API (Flask):

bash
Copy
Edit
python app_flask.py
    Endpoints Overview
POST /classify_email → Classifies email into category.

POST /mask_email → Applies PII masking on input text.

GET / → Welcome route or health check.

Check /docs (FastAPI) for auto-generated API docs.

   Deployment
This project is compatible with:

Hugging Face Spaces (via app.py)

Render, Railway, or any Docker-based service

 Author
Siddharthan R
23rd April 2025
Developed as part of an internship assignment at [Company Name].

 License
MIT License — feel free to use and adapt this project.

yaml
Copy
Edit

---

Would you like me to:
- Insert this directly into your project?
- Customize with Hugging Face deployment tips or an example API request?

Let me know and I’ll update it right away!
