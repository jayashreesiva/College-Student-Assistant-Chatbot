# 🎓 College Student Assistant Chatbot

An **AI-based College Student Assistant Chatbot** developed using **Python and Machine Learning** in Google Colab.

The chatbot helps students get quick answers to common college-related questions such as **departments, academics, facilities, placements, library, hostel, transport, examinations, scholarships, admissions, and student services**.

## 📌 Project Overview

The College Student Assistant uses a **TF-IDF-based text similarity approach** to understand a student's question and find the most relevant information from a college knowledge base.

### Example

**Student:**

> What facilities are available in the college?

**Chatbot:**

> The college provides facilities such as laboratories, library, classrooms, transportation, hostel facilities, and other student services.

---

## 🎯 Objectives

* Provide quick answers to common student queries.
* Create a simple college information chatbot.
* Use Machine Learning for text similarity.
* Reduce the need to manually search through college information.
* Provide an interactive chatbot experience.
* Handle unknown questions safely instead of generating random answers.

---

## 🛠️ Technologies Used

| Technology        | Purpose                             |
| ----------------- | ----------------------------------- |
| Python            | Main programming language           |
| Google Colab      | Development environment             |
| Pandas            | Dataset and data processing         |
| NumPy             | Numerical operations                |
| Scikit-learn      | Machine Learning                    |
| TF-IDF            | Convert text into numerical vectors |
| Cosine Similarity | Find the most relevant information  |
| Matplotlib        | Visualization                       |
| Seaborn           | Data visualization                  |

---

## 🧠 Machine Learning Approach

This project uses **content-based text similarity**.

### Workflow

```text
Student Question
       ↓
Text Cleaning
       ↓
TF-IDF Vectorization
       ↓
Cosine Similarity
       ↓
Compare with College Knowledge Base
       ↓
Find Most Relevant Information
       ↓
Similarity Threshold Check
       ↓
Chatbot Response
```

---

## 📚 Knowledge Base

The chatbot contains information related to different college categories:

* 🏫 College
* 🎓 Departments
* 📖 Academics
* 🏢 Facilities
* 💼 Placements
* 👨‍🎓 Student Services
* 📚 Library
* 📝 Admissions
* 📋 Examinations
* 🏠 Hostel
* 🚌 Transport
* 💰 Scholarships

The knowledge base is stored and processed using a Pandas DataFrame.

---

## 🔍 How the Chatbot Works

### 1. Text Cleaning

The user's question is converted into lowercase and unnecessary characters are removed.

### 2. TF-IDF Vectorization

TF-IDF converts the questions and knowledge-base information into numerical vectors.

**TF-IDF** stands for:

> Term Frequency – Inverse Document Frequency

It gives higher importance to useful words and lower importance to commonly occurring words.

### 3. Cosine Similarity

The chatbot compares the student's question with the stored knowledge-base information using **cosine similarity**.

The similarity score helps determine which information is most relevant.

### 4. Similarity Threshold

A threshold is used to avoid returning unrelated answers.

If the similarity is too low, the chatbot responds that the information is not available in its current knowledge base.

---

## 💬 Example Questions

You can test the chatbot with questions such as:

```text
What departments are available?

Tell me about the library.

What facilities does the college have?

How can I apply for admission?

Does the college provide hostel facilities?

What placement services are available?

Tell me about scholarships.

How does the examination system work?

Is transportation available?

What student services are provided?
```

---

## 📊 Features

### ✅ College Information Search

Find information from the college knowledge base.

### ✅ Machine Learning-Based Matching

Uses TF-IDF and cosine similarity instead of simple keyword matching.

### ✅ Similarity Score

Shows how closely the student's question matches the stored information.

### ✅ Unknown Query Handling

If the chatbot cannot find a sufficiently relevant answer, it does not randomly generate information.

### ✅ Conversation History

The project stores previous questions and responses during the chatbot session.

### ✅ Interactive Chatbot

Students can continuously enter questions and receive responses.

### ✅ Dataset Export

The knowledge base and chatbot results can be saved as CSV files.

---

## 📁 Project Files

After running the notebook, the project can contain:

```text
College_Student_Assistant/
│
├── College_Student_Assistant.ipynb
├── college_knowledge_base.csv
├── college_tfidf_vectorizer.pkl
├── chatbot_sample_results.csv
└── college_student_assistant_summary.csv
```

### File Description

| File                                    | Description                 |
| --------------------------------------- | --------------------------- |
| `College_Student_Assistant.ipynb`       | Main Google Colab notebook  |
| `college_knowledge_base.csv`            | College information dataset |
| `college_tfidf_vectorizer.pkl`          | Saved TF-IDF vectorizer     |
| `chatbot_sample_results.csv`            | Sample chatbot predictions  |
| `college_student_assistant_summary.csv` | Project summary             |

---

## 🚀 How to Run

### Step 1: Open Google Colab

Open the notebook:

```text
College_Student_Assistant.ipynb
```

### Step 2: Run the cells

Run the notebook cells from top to bottom.

### Step 3: Install required libraries

```python
!pip install -q pandas numpy scikit-learn matplotlib
```

### Step 4: Test the chatbot

Enter a question such as:

```text
What departments are available?
```

The chatbot searches the knowledge base and returns the most relevant response.

---

## 📈 Machine Learning Model

This project uses:

**TF-IDF Vectorization + Cosine Similarity**

It is a lightweight and explainable approach for a small college information knowledge base.

No external Large Language Model is required for the basic chatbot.

---

## 🔮 Future Enhancements

The project can be improved by adding:

* Voice input and speech recognition
* Text-to-speech responses
* Multilingual support
* Larger college knowledge base
* Real college website data
* FAQ document/PDF processing
* Retrieval-Augmented Generation (RAG)
* Large Language Model integration
* Web-based chatbot interface
* Student login system
* Personalized student assistance
* College timetable integration
* Placement notification system

---

## 🎓 Learning Outcomes

Through this project, the following concepts were practiced:

* Python programming
* Pandas data processing
* Text preprocessing
* Natural Language Processing basics
* TF-IDF
* Cosine similarity
* Machine Learning classification/search concepts
* Chatbot development
* Dataset management
* Model/vectorizer saving
* Google Colab
* GitHub project organization

---

## 📌 Project Type

**Domain:** Artificial Intelligence / Machine Learning / NLP

**Project Type:** Educational Chatbot

**Development Platform:** Google Colab

**Programming Language:** Python

**Machine Learning Technique:** TF-IDF + Cosine Similarity

---

## 👩‍💻 Author

**Jaya Shree S**

B.E. Computer Science and Engineering

Prathyusha Engineering College

---

## ⭐ Conclusion

The **College Student Assistant Chatbot** provides a simple and practical way for students to obtain information about college-related services.

By combining **text preprocessing, TF-IDF vectorization, and cosine similarity**, the system can identify relevant information from a structured college knowledge base and provide appropriate responses to student queries.
