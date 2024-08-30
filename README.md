# CODE-MANGA_Dhaanish-Assessment-Platform-



---

# Assessment Platform

## Overview
The **Assessment Platform** is designed to efficiently evaluate candidates through customizable assessments powered by advanced AI technologies. The platform provides real-time AI proctoring, secure data management, and comprehensive post-assessment reporting. It supports a seamless and scalable experience for administrators, educators, and candidates alike.

## Features
- **Custom Question Upload:** Supports manual upload of various question types (MCQs, short answers, coding challenges).
- **AI-Powered Proctoring:** Real-time monitoring with advanced features like gaze detection and device tracking to prevent dishonest behaviors.
- **Data Security:** Encryption of candidate data and strict access control measures.
- **Scalability:** Capable of handling large candidate volumes with automated monitoring and reporting.
- **Comprehensive Reporting:** Detailed reports for assessment and proctoring, offering insights into candidate performance and activities.

## Key Modules

### 1. **Custom Question Upload**
This module allows administrators and educators to upload customized questions in different formats such as:
- **Multiple Choice Questions (MCQ)**
- **Short Answer Questions**
- **Coding Challenges**

<img src="analyze.png">

It supports bulk upload and provides flexibility in content creation to ensure assessments are tailored to specific job roles.

### 2. **AI-Powered Proctoring**
The platform uses real-time AI-powered proctoring, which includes:
- **Facial Recognition:** Verifying the identity of candidates.
- **Eye Tracking:** Detecting gaze diversion and other suspicious activities.
- **Motion Detection:** Monitoring for unusual behavior during the assessment.
- **Audio Analysis:** Capturing and analyzing ambient sounds to detect unauthorized assistance.

<img src="configure-general.png">

### 3. **Data Security**
Ensures end-to-end encryption of candidate data and assessment content. The platform uses the following measures to ensure data privacy:
- Secure access control.
- Encrypted storage and transmission.
- Regular audits and compliance with data privacy regulations.

<img src="configure-grading.png">

### 4. **Scalability and Performance**
The platform is built to handle large-scale assessments with automated processes that reduce manual intervention:
- Supports concurrent assessments for a large number of candidates.
- Scalable cloud infrastructure for seamless performance even during peak usage times.

<img src="configure-results.png">

## Stakeholders
1. **Primary Stakeholders**
   - **Candidates:** Participate in assessments and receive real-time feedback.
   - **Educators/Instructors:** Design assessments, upload questions, and review performance reports.

<img src="create.png">

2. **Secondary Stakeholders**
   - **IT/Security Teams:** Ensure platform security and reliability.
   - **Platform Developers:** Continuously enhance features based on user feedback.

<img src="new ques.png">

## User Roles
- **Candidates:** Complete assessments with AI monitoring.
- **Educators/Instructors:** Upload and manage assessment content, track performance.
- **Administrators:** Oversee platform operations, manage users, ensure system security.

<img src="preview.png">

## Process Flow
### Candidates:
1. **Registration and Login**
2. **System Check**
3. **Start Assessment** with AI Proctoring
4. **Submit and Review Results**

<img src="profile.png">

### Educators/Instructors:
1. **Login and Dashboard Access**
2. **Create/Upload Assessment Content**
3. **Monitor Performance and Feedback**

<img src="publish.png">

### Administrators:
1. **User Management**
2. **Assessment Setup and Monitoring**
3. **Generate Reports and Manage Security**

<img src="results.png">

## Algorithms and AI
- **Natural Language Processing (NLP):** For text classification and sentiment analysis.
- **Machine Learning:** To predict scores and categorize responses.
- **AI Proctoring:** Using facial recognition, eye-tracking, and sound anomaly detection to monitor candidates in real-time.

<img src="s-dashboard.png">

## Reporting
- **Assessment Reports:** Overview of test scores, individual performance, and frequently missed questions.
- **Proctoring Reports:** Summary of flagged incidents and detailed proctoring logs.
- **User Activity Reports:** Track user engagement and activities for auditing and compliance purposes.

<img src="s-ongoing test.png">

## System Requirements
To use the platform efficiently, the following system requirements are recommended:


<img src="s-profile.png">

### For Candidates:
- **Browser:** Latest versions of Chrome, Firefox, or Safari.
- **Hardware:** Webcam and microphone enabled.
- **Internet:** Minimum speed of 5 Mbps.
- **OS:** Windows 10 or later, macOS 10.15 or later.

<img src="s-test saved.png"><img src="s-test started.png">

### For Educators/Administrators:
- **Browser:** Latest versions of Chrome, Firefox, or Safari.
- **Hardware:** No additional requirements beyond a standard computer.
- **Internet:** Minimum speed of 10 Mbps for monitoring multiple assessments.

 <img src="s-tests.png"> <img src="s-view result.png">

## Installation Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Dineshkumar12300/CODE-MANGA_Dhaanish-Assessment-Platform-.git
   cd assessment-platform
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Setup the Database:**
   ```bash
   python manage.py migrate
   ```

4. **Run the Application:**
   ```bash
   python manage.py runserver
   ```

5. **Access the Platform:**
   Open your browser and navigate to `http://localhost:8000`.

## API Integration

The platform supports integration with third-party systems via a RESTful API. The following endpoints are available:

- **/api/upload-questions** - Upload questions in bulk.
- **/api/monitor-assessments** - Real-time monitoring of assessments.
- **/api/generate-reports** - Generate post-assessment and proctoring reports.

### Example API Request:
```bash
POST /api/upload-questions
Content-Type: application/json
Authorization: Bearer <token>

{
   "questions": [
      {
         "type": "MCQ",
         "question_text": "What is the capital of France?",
         "options": ["Paris", "London", "Berlin", "Madrid"],
         "correct_option": "Paris"
      }
   ]
}
```

### API Documentation:
Detailed API documentation is available [here](API_DOCS.md).

## Known Issues
- **Browser Compatibility:** Some older versions of browsers may not fully support the AI proctoring features. Please ensure candidates are using the latest browser versions.
- **Audio Detection Sensitivity:** In environments with constant background noise, the audio detection system may produce false positives.

## Roadmap
Planned features for future releases include:
- **Mobile Support:** Enabling candidates to take assessments on mobile devices.
- **Multilingual Support:** Expanding the platform to support additional languages.
- **Advanced Reporting:** Enhanced analytics for candidate performance and proctoring efficiency.

## How to Contribute
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This README provides a comprehensive guide covering all the essential aspects of the platform, including features, user roles, algorithms, installation, API integration, known issues, and future roadmap.
