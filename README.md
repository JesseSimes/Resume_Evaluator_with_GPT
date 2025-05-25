## 🧭 **📍Resume Evaluator with GPT**

### 🔹 **Week 1: Resume Extraction + Parsing**

> ✅ Goal: Extract structured data from resume files (PDF/DOCX)

**Tasks:**

* Collect sample resumes in different formats (PDF, DOCX).
* Implement file upload and text extraction:

  * `PyMuPDF`, `pdfminer.six` or `pdfplumber` for PDFs
  * `python-docx` for DOCX
* Clean and normalize extracted text.
* Optional: Extract structured fields like name, email, skills, education, etc.

**Deliverable:** `parser.py` that outputs clean resume text.

---

### 🔹 **Week 2: Prompt Engineering + GPT Integration**

> ✅ Goal: Design and test prompts for evaluating resumes using GPT

**Tasks:**

* Identify key evaluation criteria:

  * Relevance of skills
  * Formatting and clarity
  * Experience strength
  * Education background
  * ATS compatibility (keyword usage)
* Write prompt templates (few-shot or zero-shot) in a separate `prompts/` folder.
* Create `evaluator.py` to:

  * Load the resume text
  * Insert it into the prompt
  * Call the GPT model via OpenAI API or LangChain

**Deliverable:** Functional GPT-based evaluator returning structured feedback.

---

### 🔹 **Week 3: Scoring System + Feedback Generation**

> ✅ Goal: Convert GPT feedback into quantifiable scores and useful tips

**Tasks:**

* Parse GPT output into a structured format (using regex/JSON parsing).
* Design scoring logic:

  * Use GPT response or rule-based system to assign scores (0–100) for each category.
* Create `scorer.py` to:

  * Take GPT output
  * Assign scores per section
  * Summarize and recommend improvements

**Deliverable:** Resume scorecard + feedback report in text or JSON format.

---

### 🔹 **Week 4: User Interface + Report Generator**

> ✅ Goal: Build a minimal app interface and generate downloadable reports

**Tasks:**

* Build a simple Streamlit or Gradio UI:

  * File upload
  * Display parsed content
  * Show GPT feedback and scores
* Optionally allow user role (e.g., "Developer Role") for role-specific evaluation.
* Export report as PDF using `fpdf` or `reportlab`.

**Deliverable:** MVP resume evaluation app with downloadable report.

---

### 📦 Final Deliverables:

* ✅ Full codebase (with comments and README)
* ✅ Demo video (optional)
* ✅ Evaluation reports for sample resumes
* ✅ A write-up / blog summarizing the build process

---

### 🧠 Skills You’ll Build:

* Prompt engineering techniques
* Resume parsing with Python NLP
* LLM integration with APIs
* Scoring logic & data structuring
* Streamlit or Gradio UI design


