# Interactive Quiz App with Google Gemini

This project creates an interactive quiz application that leverages the power of Google Gemini's large language model (LLM) to dynamically generate multiple-choice questions.  The quiz is built using React and fetches data from a JSON file containing a detailed curriculum.

## Table of Contents

*   [Features](#-features)
*   [How it Works](#-how-it-works)
*   [Technology Stack](#-technology-stack)
*   [Setup](#%EF%B8%8F-setup)
    *   [1. Clone the repository](#1-clone-the-repository)
    *   [2. Install dependencies](#2-install-dependencies)
    *   [3. Set API Key](#3-set-api-key)
    *   [4. Run the app](#4-run-the-app)
*   [Important Note](#%EF%B8%8F-important-note)
*   [Future Improvements](#-future-improvements)


## 🚀 **Features:**

*   **Dynamic Question Generation:** Uses Google Gemini to create unique multiple-choice questions based on selected modules and topics from a provided curriculum.  No more static quizzes! 🎉
*   **Curriculum-Based:**  Fetches data from a JSON file ( `FinalYearBTechComputerEngineering.json` ) representing a curriculum.  Easily adaptable to different subjects and courses. 📚
*   **Semester and Subject Selection:**  Users choose the semester and subject they want to be quizzed on. 🗓️
*   **Multiple Module Selection:** Users can select multiple modules for a more comprehensive quiz experience. 🗂️
*   **Check All/Uncheck All:**  A convenient button to check/uncheck all modules at once. ☑️
*   **Immediate Feedback:**  Provides instant feedback on the correctness of user's answers with a clear score. ✅❌
*   **Shuffled Questions and Options:** For a more engaging experience, both questions and answer options within each question are randomly shuffled. 🔀


## 🤔 **How it Works:**

1.  **Data Fetching:** The app loads the curriculum data from the JSON file on initialization.
2.  **User Selection:**  Users select the semester, subject, and modules they'd like to be quizzed on.
3.  **Prompt Generation:** Based on user selections, a prompt is dynamically generated and sent to the Google Gemini API.
4.  **API Call:** The app calls the Google Gemini API (requires a valid API key).
5.  **Question Generation:**  Gemini generates multiple-choice questions, including correct and incorrect answers.
6.  **Result Display:** The app displays the questions with randomized options, allowing the user to select answers.  Once submitted, it shows the results with feedback on correctness.
7.  **Shuffling:** The questions and answer options are shuffled for each quiz session.

## 💻 **Technology Stack:**

*   **Frontend:** React
*   **LLM:** Google Gemini
*   **State Management:** `useState`, `useEffect`, `useMemo`, `useCallback`

## ⚙️ **Setup:**

### 1. Clone the repository:
```bash
git clone <repository_url>
```

### 2. Install dependencies:
```bash
npm install
```

### 3. Set API Key:
Replace `process.env.NEXT_PUBLIC_API_KEY` with your actual Google Gemini API key. You will need to obtain this from Google Cloud.  **This is crucial for the app to function.** 🔑

### 4. Run the app:
```bash
npm run dev
```

## ⚠️ **Important Note:**

This application requires a Google Gemini API key. You must obtain one from Google Cloud before running the application.


## ✨ **Future Improvements:**

*   **Persistent Storage:** Save user scores and progress.
*   **Difficulty Levels:** Offer different difficulty levels for questions.
*   **Advanced Question Types:** Include more varied question formats.
*   **Progress Tracking:** Add a progress bar to track the user's progress.


This project is a great example of how to integrate LLMs into interactive applications.  Enjoy! 😄

