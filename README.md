## 🚗 AutoQuoteBot: Automated Insurance Quote Testing 🛠️

![Robot Framework](https://img.shields.io/badge/RobotFramework-3.2.2-green)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)

> **Automated testing project for an insurance web application using Robot Framework and CI/CD.**

AutoQuoteBot is a test automation suite developed with **Robot Framework** for automating the process of creating and verifying insurance quotes on a sample automobile insurance application. This project is CI/CD-ready, enabling smooth integration with platforms like **GitHub Actions** for continuous testing and quality assurance. 

### 📁 Project Structure
```plaintext
InsuranceRobotCICD/
│
├── tests/
│   ├── test_cases.robot            # Main test suite for creating insurance quotes
│   └── resources/
│       ├── keywords.robot          # Reusable custom keywords
│       └── variables.robot         # Reusable variables (e.g., URLs, browser settings)
│
├── .github/
│   └── workflows/
│       └── robot-tests.yml         # GitHub Actions CI/CD workflow file
│
├── output/                         # Directory for test output, logs, and reports
│
├── requirements.txt                # List of project dependencies
│
└── README.md                       # Project documentation
```

### 🚀 Features
- **Automated Testing:** Automates the steps to generate and verify an insurance quote.
- **Reusable Keywords and Variables:** Modular keywords and variables for flexibility and easy maintenance.
- **CI/CD Ready:** Integrated GitHub Actions workflow to automate testing on each code push.
- **Cross-Browser Compatibility:** Supports different browsers for testing with minimal configuration.

### 🛠️ Prerequisites
Before you begin, ensure you have the following installed:

- **Python** (>= 3.8) 
- **pip** (Python package manager)
- **Node.js** (for Browser library support)

### 📥 Installation

1. **Clone the repository**:
     ```bash
     git clone https://github.com/khizraghaffarkk/InsuranceRobotCICD.git
     cd InsuranceRobotCICD
     ```

2. **Install dependencies**:
     ```bash
     pip install -r requirements.txt
     ```

3. **Install Browser Library dependencies**:
     ```bash
     rfbrowser init
     ```

### 🧩 Running the Tests
To execute the test suite locally, run:
```bash
robot tests/test_cases.robot
```
#### Viewing Results
After the tests complete, open `output/log.html` or `output/report.html` to view detailed logs and reports.

### 🤖 CI/CD with GitHub Actions
This project includes a GitHub Actions workflow for continuous integration and testing on each push. The configuration file is located at:

#### .github/workflows/robot-tests.yml
The CI/CD workflow will:

1. Set up Python and dependencies.
2. Run the test suite.
3. Save test results as artifacts for review.

### 🔑 Key Project Files
- `test_cases.robot:` Main test file containing test cases for generating insurance quotes.
- `keywords.robot:` Contains reusable keywords for maintaining modular tests.
- `variables.robot:` Stores reusable variables like browser type, URLs, and input data.
- `.github/workflows/robot-tests.yml:` GitHub Actions configuration file for automating test execution.
