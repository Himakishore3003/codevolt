

# CodeVolt: AI-Powered EV Diagnostics
[![Ask DeepWiki](https://devin.ai/assets/askdeepwiki.png)](https://deepwiki.com/Himakishore3003/codevolt)

CodeVolt is a comprehensive web-based platform designed to simplify Electric Vehicle (EV) diagnostics through the power of artificial intelligence. It offers two primary tools: an AI-powered flashcard generator for instant issue diagnosis and a data analysis tool to evaluate EV performance from CSV data.

This project leverages Google's Gemini API for intelligent text and analysis generation and Eden AI for creating relevant diagnostic imagery, providing users with an intuitive and powerful diagnostic experience.

## Features

### 1. Diagnostic Flashcard Generator (`index.html`)
- **Instant Diagnosis:** Enter any EV problem or error code to receive immediate, AI-generated diagnostic information.
- **Customizable Output:** Specify the number of flashcards (1-20) and the content type (text only, text with icons, or text with images).
- **Rich Visuals:** Automatically generates relevant images and icons for flashcards using Eden AI to aid visual understanding.
- **Stylish Templates:** Choose from multiple design templates (Classic, Modern, Vibrant, Gradient) and color schemes to personalize your learning experience.
- **Light & Dark Mode:** A theme toggle for comfortable viewing in any lighting condition.

### 2. EV Data Analyzer (`index1.html`)
- **CSV Data Upload:** Analyze your EV's performance by uploading a CSV file with relevant metrics.
- **Automated KPI Calculation:** The tool automatically parses the data and calculates key metrics such as average speed, battery health, payload weight, battery temperature, and more.
- **AI-Powered Insights:** Uses the Gemini API to analyze the calculated metrics, compare them with industry standards, and provide a concise, easy-to-understand summary.

## Tech Stack

- **Frontend:** HTML5, CSS3, JavaScript, Bootstrap 5
- **AI Services:**
  - **Google Gemini API:** For generating diagnostic text and data analysis.
  - **Eden AI API:** For generating images for flashcards.
- **Backend & Authentication:** Firebase (for user sign-up and login functionality).

## Getting Started

The project is entirely client-side and can be run by opening the HTML files in a web browser.

### Prerequisites
You will need API keys from the following services:
- **Google Gemini API**
- **Eden AI API**
- A **Firebase** project for user authentication.

### Installation & Configuration

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/himakishore3003/codevolt.git
    cd codevolt
    ```

2.  **Configure API Keys:**
    You must replace the placeholder API keys in the JavaScript files with your own.

    -   **For the Flashcard Generator (`script.js`):**
        Update the `GEMINI_API_KEY` and `EDEN_API_KEY` variables at the top of the file.
        ```javascript
        const GEMINI_API_KEY = "YOUR_GEMINI_API_KEY";
        const EDEN_API_KEY = "YOUR_EDEN_AI_API_KEY";
        ```

    -   **For the Data Analyzer (`ctrl.js`):**
        Update the `GEMINI_API_KEY` variable at the top of the file.
        ```javascript
        const GEMINI_API_KEY = "YOUR_GEMINI_API_KEY";
        ```

    -   **For Firebase Authentication (`register.js`):**
        Replace the placeholder `firebaseConfig` object with your Firebase project's configuration.
        ```javascript
        const firebaseConfig = {
          apiKey: "YOUR_FIREBASE_API_KEY",
          authDomain: "YOUR_AUTH_DOMAIN",
          projectId: "YOUR_PROJECT_ID",
          storageBucket: "YOUR_STORAGE_BUCKET",
          messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
          appId: "YOUR_APP_ID"
        };
        ```

3.  **Run the application:**
    Open `index.html` or `index1.html` in your web browser to start using the application.

## Usage

### Generating Diagnostic Flashcards
1.  Navigate to `index.html`.
2.  Enter an EV problem or error code into the text area (e.g., "P0AA6 - Battery Isolation Fault").
3.  Select the desired number of cards and content type.
4.  Choose a visual template and color scheme.
5.  Click the **"Generate Flashcards"** button. The AI-generated cards will appear below.

### Analyzing EV Data
1.  Navigate to `index1.html`.
2.  Click the **"Choose File"** button and select a CSV file with your EV's performance data. The CSV should contain headers like `avg_speed_0_60_mph`, `battery_health_percent`, `payload_weight_pounds`, etc.
3.  Click the **"Analyze"** button.
4.  The application will display the calculated metrics and an AI-generated analysis of the data.

## Meet the Team

-   **Varun Kumar R:** Frontend Developer
-   **Kathari Hima Kishore:** Backend Developer
-   **Srinivasan R:** Database & Cloud
-   **Saikrishna Kumaravel:** Backend Developer
