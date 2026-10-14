# CareerPilot AI 🚀

**AI-Powered Resume Screening & Career Skill-Gap Navigator**

CareerPilot AI is a career guidance application designed to help
students and fresh graduates understand how closely their resumes match
job requirements. Users can upload a PDF resume and enter a target job
description to review a matching score, matching skills, and potential
skill gaps.

## 🎯 Problem Statement

**ED-03 --- Career and Skill-Gap Navigator**\
**Category:** EdTech

Students and fresh graduates may find it difficult to identify the
skills employers expect for a particular role and understand how their
resumes compare with those requirements. CareerPilot AI addresses this
challenge by comparing resume content with a target job description and
presenting information that can help users identify areas for
improvement.

## 💡 Our Solution

CareerPilot AI provides a web-based workflow for resume-to-job
comparison. Users enter a job title and job description, upload a PDF
resume, and review the analysis results. The application helps users
understand which relevant skills are present in their resume and which
skills may need further attention.

The matching result is intended as guidance. It is not a guarantee of
job suitability, interview selection, or employment.

## ✨ Key Features

-   **PDF Resume Upload:** Upload a resume in PDF format for analysis.
-   **Job Description Comparison:** Compare resume content with the
    requirements of a target role.
-   **Skill Matching:** Identify relevant skills found in both the
    resume and job requirements.
-   **Skill-Gap Identification:** Highlight relevant job skills that may
    be missing from the resume.
-   **Resume Matching Score:** Provide a combined score based on skill
    coverage and text similarity.
-   **TF-IDF Text Similarity:** Compare resume text with job-description
    text using a text-similarity approach.
-   **Additional Career Support:** Interview preparation, career
    guidance, learning recommendations, history, and export features
    should be described as available only where they are enabled and
    working in the submitted version.

## ⚙️ How It Works

1.  **Enter Job Details:** The user provides a job title and job
    description.
2.  **Upload Resume:** The user uploads a PDF resume.
3.  **Extract Text:** The application extracts readable text from the
    PDF.
4.  **Analyze Skills:** Resume skills are compared with skills
    identified in the job description.
5.  **Calculate Text Similarity:** TF-IDF-based analysis estimates the
    similarity between the resume and job-description text.
6.  **Display Results:** The application presents a matching score,
    matching skills, and potential skill gaps.
7.  **Review and Improve:** The user can use the results to decide which
    areas may need further learning or resume improvement.

## 🧠 Matching Approach

The current project description specifies a weighted matching approach:

-   **70% Skill Coverage:** Measures how well the resume covers the
    identified job-related skills.
-   **30% Text Similarity:** Uses TF-IDF-based similarity to estimate
    how closely the resume text relates to the job description.

The combined score is a guidance signal. It should not be treated as a
validated prediction of recruitment outcomes. Confirm these weights
against the submitted source code before presenting them as
implementation facts.

## 🛠️ Technologies Used

-   **Python** --- Application logic and text processing.
-   **Streamlit** --- Interactive web application interface.
-   **Scikit-learn** --- TF-IDF vectorization and text similarity, if
    confirmed in the submitted dependencies.
-   **PDF text-extraction library** --- Used to extract text from
    uploaded resumes; name the exact package listed in the project
    dependencies.
-   **SQLite** --- Local analysis-history storage, where implemented in
    the submitted version.
-   **Groq API** --- Optional AI-powered functionality, where configured
    and enabled.
-   **Git and GitHub** --- Version control and source-code hosting.
-   **Streamlit Community Cloud** --- Application deployment.

Only list technologies and features that are actually present in the
submitted code. Update this section if the repository's dependency files
or implementation differ.

## 🚧 Challenges Faced

-   Extracting useful text from PDF resumes.
-   Identifying relevant skills in resumes and job descriptions.
-   Comparing resume content with job requirements.
-   Combining skill coverage and text similarity into a single score.
-   Managing application configuration and optional API-based features.
-   Deploying the application for a public demonstration.

## 📚 Learnings

Through this project, the team explored:

-   Resume text extraction and preprocessing.
-   Skill matching and text-similarity techniques.
-   Applying TF-IDF to a practical career-related problem.
-   Building an interactive application with Streamlit.
-   Integrating software libraries and optional AI services.
-   Managing source code with Git and GitHub.
-   Deploying a web application for public access.

## 🔮 Future Improvements

Potential future improvements include:

-   Structured student profiles containing courses, projects, skills,
    and interests.
-   Verified learning resources tailored to identified skill gaps.
-   Portfolio-project recommendations for target roles.
-   Milestone-based progress tracking.
-   Support for additional resume formats and improved skill extraction.
-   Evaluation of matching quality across a broader set of resumes and
    job descriptions.

These are future possibilities, not claims about features already
implemented.

## 🤖 AI and Open-Source Usage

The project uses software libraries and development tools as part of its
implementation. The team should disclose the specific AI coding tools,
models, APIs, and open-source packages actually used.

-   **Text analysis:** Scikit-learn / TF-IDF, if confirmed in the
    project dependencies.
-   **AI API:** Groq API, if configured and used in the submitted
    application.
-   **Other dependencies:** List the exact PDF-processing package and
    other libraries from the project's dependency files.
-   **AI-assisted development:** Add the names of the AI tools used by
    the team and briefly state how they were used.

Do not include API keys, passwords, tokens, `.env` contents, or other
secrets in this README or in the repository.

## 👥 Team Members

**Team Name:** CYBER WOLVES 🐺

-   **Ashfaque Ahmed** --- K24SW035
-   **Hasnain Ali** --- K24SW038
-   **Niaz Bhayo** --- K24SW045

## 🔗 Project Links

-   **GitHub Repository:** [CareerPilot
    AI](https://github.com/ashfaque-ahmed78/CareerPilot-AI)
-   **Live Application:** [Open CareerPilot
    AI](https://careerpilot-ai-qpgmzurksxjg2kddxqevkl.streamlit.app/)
-   **Demo Video:** [Watch the Project
    Demo](https://drive.google.com/file/d/1vAO8RGDi9eDj3aIKR4BlIFpgtcu-QfIz/view?usp=drive_link)

## 🎯 Project Goal

Our goal is to help students and fresh graduates better understand job
requirements, recognize potential skill gaps, and prepare more
effectively for their career journeys.

**CareerPilot AI --- Understand Your Skills. Discover Your Gaps. Prepare
for Your Career.**
