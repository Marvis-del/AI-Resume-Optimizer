# JobAI – AI Resume Optimizer & Cover Letter Generator

**JobAI** is a free, web-based tool that helps job seekers (especially in Nigeria) optimize their resumes and generate tailored cover letters quickly. It analyzes your resume against a job description, calculates an ATS match score, suggests missing keywords, rewrites bullet points, and creates a professional cover letter — all powered by Groq's fast AI models.

Perfect for applying to Nigerian banks (GTBank, Zenith, Access), fintech companies (Paystack, Flutterwave, Moniepoint), remote global roles, or any competitive position where ATS rejection is common.

### Features
- Upload your resume (PDF) and paste the job description
- Instant ATS compatibility score using semantic similarity
- Recommended Nigeria-relevant keywords to add (e.g., "KYC", "fintech API", "SQL", "Agile")
- AI-rewritten, stronger bullet points aligned with the JD
- Full tailored cover letter (350–450 words) with professional tone
- Tone customization: Professional, More Confident, Shorter, Pidgin-friendly
- Download cover letter as .docx and improved bullets as .txt
- Clear/reset functionality for multiple tests

### Live Demo
Try it here:  
https://justmarvis29-jobai-resume-optimizer.hf.space  
(or your Streamlit Cloud link once deployed)

### Tech Stack
- **Frontend & Backend**: Streamlit (Python-based web app)
- **PDF Parsing**: PyMuPDF (fitz)
- **Semantic Similarity / ATS Scoring**: sentence-transformers (`all-MiniLM-L6-v2`)
- **AI Generation**: Groq (Llama-3.3-70B-Versatile)
- **Document Export**: python-docx
- **Environment Management**: python-dotenv

### How to Run Locally
1. Clone the repo:
   ```bash
   git clone https://github.com/JustMarvis29/jobai-resume-optimizer.git
   cd jobai-resume-optimizer

### Create virtual environment & install dependencies:Bashpython -m venv .venv
 ```source .venv/bin/activate   # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
Add your Groq API key:
Create .env file:textGROQ_API_KEY=your_new_key_here
Run the app:Bashstreamlit run streamlit_app.py
   ```bash
   git clone https://github.com/JustMarvis29/jobai-resume-optimizer.git
   cd jobai-resume-optimizer
