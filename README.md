# Chatbot Development and Deployment Guide

## 1. Introduction:
A chatbot is a software application designed to simulate human-like conversations. They are widely used in tasks such as booking tickets, answering questions, online shopping, and more.

---

## 2. Development Environment Setup:
### Required Libraries:
- **nltk**
- **sklearn**
- **ssl**
- **streamlit**

### Specific Packages:
- **punkt**
- **wordnet**

---

## 3. Steps to Upload to GitHub:
1. **Login to your GitHub account** and create a new repository.
2. **Add your required files**:
   - Python file (e.g., `file.py`)
   - JSON file (e.g., `file.json`)
   - `requirements.txt` listing all external libraries to be installed.

---

## 4. Steps to Run the Chatbot Code:

### Case 1: Running in a Specific Environment
1. Open CMD or PowerShell.
2. Install the required packages by running the following commands:
   ```bash
   pip install nltk
   pip install scikit-learn
   pip install streamlit
   ```
3. To view your Streamlit app in the browser, run the following command:
   ```bash
   streamlit run path\project.py
   ```
   *(Replace `path` with the actual file path and `project` with your project name.)*

### Case 2: Testing a Python File from GitHub in Terminal
#### I. Clone the Repository:
1. Open your terminal or CMD/PowerShell.
2. Navigate to the directory where you want to clone the repo:
   ```bash
   cd path/to/your/directory
   ```
3. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
   **Example:**
   ```bash
   git clone https://github.com/khirishwanth/Rule_based_chatbot.git
   ```
   *This downloads the repository to your local machine.*

#### II. Set Up a Virtual Environment (Optional but Recommended):
1. Create a virtual environment:
   ```bash
   python -m venv chatbot_env
   ```
2. Activate the virtual environment:
   - **Linux/Mac:**
     ```bash
     source chatbot_env/bin/activate
     ```
   - **Windows (CMD/PowerShell):**
     ```bash
     chatbot_env\Scripts\activate
     ```

#### III. Install Required Packages:
Ensure the `requirements.txt` file is in the repository.
```bash
pip install -r requirements.txt
```

#### IV. Run the Python File:
- **For Streamlit apps:**
  ```bash
  streamlit run chatbot.py
  ```
- **For non-Streamlit apps:**
  ```bash
  python chatbot.py
  ```

#### V. Exit the Virtual Environment:
```bash
deactivate
```

### Case 3: Terminal Unexpectedly Closes
- Repeat the steps from **Case 2**, except for cloning the repository.

### Case 4: Update Virtual Environment After GitHub Updates
- This command is used when we want the changes done directly in the github to get reflected in the terminal
```bash
git pull origin main
```

---

## 5. Steps to Deploy on Streamlit:
1. Go to **Streamlit Cloud**.
2. **Log in with your GitHub account** (if not already connected).
3. Click **"New App"** (top-right corner).
4. Select the GitHub repository with your chatbot project.
5. **Branch:** Choose `main` (or your working branch).
6. **Main File Path:** Enter the path to the Python file (e.g., `chatbot.py`).
7. Click the **Deploy** button.





