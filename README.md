# 🧪 Singlish to Sinhala Translator – Test Automation

## 📌 Overview
        This project is an automated testing tool for a **Singlish to Sinhala transliteration system** using the Pixelssuite Chat Translator.

        The script reads test cases from an Excel file, sends inputs to the web interface, captures outputs, and validates results automatically.

---

## 🚀 Features

        - 📄 Reads test cases from Excel (`.xlsx`)
        - 🌐 Automates frontend testing using Playwright
        - 🔄 Sends Singlish input to the translator
        - 📥 Captures Sinhala output
        - ✅ Compares Expected vs Actual results
        - 📊 Writes results (PASS/FAIL) back to Excel
        - 🔁 Retry mechanism for stability
        - ⚠️ Handles UI/API errors gracefully

---

## 🛠️ Technologies Used

        - Python
        - Playwright
        - OpenPyXL
        - Requests

---

## 📂 Project Structure
    # IT23830264

    project-folder/
    │
    ├── test_automation.py
    ├── Assignment 1 - Test cases.xlsx
    └── README.md


---

## ⚙️ Installation

### 1️⃣ Install Python
Make sure Python is installed:
    ```bash
    python --version

2️⃣ Install dependencies

    pip install playwright openpyxl requests

3️⃣ Install Playwright browsers

    playwright install

▶️ How to Run
🔹 Basic command

        python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator"

Full command (recommended)

        python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 2000 --type-delay-ms 50 --slow-mo-ms 50 --retries 1 --retry-wait-ms 500 --save-every 1

📊 Output

        The script updates the Excel file with:

        Column	Description
        Actual Output	Output from system
        Status	PASS / FAIL