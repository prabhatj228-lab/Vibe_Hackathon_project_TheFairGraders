# Vibe_Hackathon_project_TheFairGraders
Our web app grades student answer sheets using a model answer key. It offers three grading modes—strict, standard, and mentor-based—and provides a score (0–10), similarity with the model answer, and feedback, reducing human bias and enabling diverse grading perspectives.
The Fair Grader: A Hybrid AI Grading Application

The Fair Grader is a powerful, browser-based application designed to assist educators by providing automated, flexible, and nuanced grading for student answers. It combines the semantic understanding of generative AI with the objective scoring of classical NLP algorithms to deliver a "hybrid" grade.

This tool accepts questions, model answers, and student answers in either image or text format and generates a detailed evaluation for each question, complete with a score, qualitative feedback, and a keyword similarity check.

Key Features

Hybrid Grading System: Each answer receives two scores:

AI Grade (1-10): A semantic grade from the Gemini API that evaluates the meaning, context, and understanding of the student's answer.

Similarity Score (0-1.0): An objective, mathematical score based on TF-IDF (Term Frequency-Inverse Document Frequency), which measures the keyword and term overlap with the model answer.

Flexible Inputs (Image & Text): Users are not locked into one format. For questions, model answers, and student answers, you can either:

Upload an image (like a photo of a handwritten sheet or a screenshot).

Paste or type raw text directly into a text area.

Customizable Grader Personas: Go beyond a single grade by selecting the style of feedback you want.

Balanced Grader: The standard, fair, and constructive default.

Strict Grader: A meticulous persona that penalizes errors more heavily and provides formal feedback.

Mentor Grader: An encouraging persona that uses "I" statements, praises effort, and frames mistakes as learning opportunities.

Custom Persona: Write your own instructions (e.g., "Grade as a sarcastic pirate") for limitless feedback styles.

Advanced AI Prompting: Utilizes Chain of Thought (CoT) system prompts to guide the AI through a logical, step-by-step process for both data extraction and evaluation, significantly improving accuracy.

Modern, Responsive UI:

Built with Tailwind CSS for a clean, professional, and mobile-friendly design.

Includes animated file drop-zones, image previews, and loading spinners.

Results are displayed in beautifully animated cards that fade in one by one.

Technology Stack

Frontend: HTML5, Tailwind CSS

Core Logic: Vanilla JavaScript (ES6+)

AI & Vision: Google Gemini API (gemini-2.5-flash-preview-09-2025)

Used for both OCR (reading text from images) and advanced reasoning (grading, feedback).

NLP Algorithm: A from-scratch JavaScript implementation of TF-IDF (Term Frequency-Inverse Document Frequency) and Cosine Similarity to replicate the functionality of Python libraries like NLTK and Scikit-learn.

How to Use

Get an API Key: Generate a free Gemini API key at Google AI Studio.

Paste Your Key: Paste the API key into the "Enter Your Gemini API Key" field.

Provide Inputs (x3): For the "Question Paper," "Official Answer Key," and "Student's Answer Sheet," either upload an image or paste the corresponding text.

Select a Persona: Choose one of the grader personas from the dropdown, or select "Custom Persona" and write your own.

Grade: Click the "Grade Answers" button. The app will show its progress (e.g., "Step 1/5: Reading inputs...") and then display the full results.
