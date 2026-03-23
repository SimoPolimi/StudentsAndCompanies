# 🎓💼 Students & Companies (S&C)

**Students & Companies (S&C)** is an integrated platform designed to connect university students with companies offering internships. The system addresses the complexities of finding the right match by simplifying the search, application, and management process, while also allowing universities to monitor and support their students. 

This project was created for the **Software Engineering 2** course at **Politecnico di Milano**.

---

## 📄 Deliverables

The core of this project is based on the following official documents and formal models, which define the system's requirements, architecture, and behavior:

* 📘 [**RASD (Requirement Analysis and Specification Document)**](DeliveryFolder/RASDv2.pdf): Details the problem domain, functional and non-functional requirements, use case models, and the formal analysis of the system.
* 📙 [**DD (Design Document)**](DeliveryFolder/DD.pdf): Outlines the system's high-level architecture, component design, deployment views, and user interface mockups.
* ⚙️ [**Alloy Model**](DeliveryFolder/alloy_SC.als): The formal specification used to verify system constraints and the contract lifecycle.

---

## ✨ Key Features

The platform offers a seamless experience tailored to three main user types:

### 🧑‍🎓 For Students
* **Search & Apply:** Search for internships using keyword filters and submit your application.
* **Recommendations:** Receive email notifications when an internship that might interest you becomes available.
* **CV Suggestions:** The system analyzes your profile and suggests improvements for your Curriculum Vitae to make it more attractive to companies.
* **Questionnaires:** Answer structured interview questionnaires provided by companies directly on the platform.

### 🏢 For Companies
* **Internship Management:** Publish new internship postings by specifying mandatory details like duration, required skills, and whether it is paid.
* **Talent Recommendations:** Receive email notifications when students with CVs matching your exact needs become available.
* **Interviews:** Propose structured questionnaires to evaluate your applicants efficiently.
* **Listing Optimization:** Receive system-generated suggestions on how to make your project descriptions more appealing.

### 🏛️ For Universities
* **Monitoring:** Keep track of the status of the internships for which your students have applied.
* **Direct Intervention:** Act as a supervisor and terminate an internship if unresolved controversies arise between the student and the company.

### 🤝 Shared Features
* **Discussions:** Users can initiate discussions with interested parties to exchange messages and resolve issues regarding an ongoing internship.
* **Feedback:** At the end of an internship, both students and companies can leave a required rating (1 to 5 stars) and an optional text comment to share their experience.

---

## ⚙️ System Architecture

The system is entirely web-based and relies on a **3-tier Client-Server architecture**. It implements the **MVC (Model-View-Controller)** pattern for high decoupling and maintainability. Client-server communication is handled through **RESTful APIs** over HTTPS.

*(Note: Add your architecture and deployment diagrams here if you export them later!)*

---

## 💻 User Interface (UI) Preview

Below is a preview of the platform's design and user flows:

### 🔐 1. Login & Authentication
Integration with the SheerID API allows secure verification of academic credentials.
![Login](Mockups/Desktop%20-%20Login.png)

### 🔍 2. Student Dashboard: Edit Profile & Search Internships
Students can easily build their profile, upload a CV, and browse internships matching their skills.
![Edit Profile](Mockups/Desktop%20-%20EditProfile.png)
![Search Internships](Mockups/Desktop%20-%20InternshipsList+Details.png)

### 📝 3. Company Dashboard: Post an Internship
Companies can create targeted postings by defining specific tags and terms.
![New Internship](Mockups/Desktop%20-%20NewInternship.png)

### 📋 4. Questionnaires & Forms
Companies can construct structured interviews, which students fill out directly via the platform.
![Questionnaire Form](Mockups/Desktop%20-%20Form.png)

### 📊 5. Monitor Internship Status
A clear visual tracker mapping the contract's lifecycle (from Pending to OnGoing, up to Expired or Interrupted).
![Ongoing Internship](Mockups/Desktop%20-%20OngoingInternship.png)

### 💬 6. Discussions & Chat
A dedicated space to resolve issues or conduct interviews via chat.
![Chat V1](Mockups/Desktop%20-%20Chat_V1.png)
![Chat V2](Mockups/Desktop%20-%20Chat_V2.png)

---

## 🛠️ Technologies Used

* **Backend & API:** RESTful Architecture.
* **Student Authentication:** Integration with the **SheerID API** to verify academic credentials and university enrollment.
* **Security:** Encrypted communications via the HTTPS protocol and strict compliance with GDPR data protection laws.
* **Formal Analysis:** Use of [**Alloy**](DeliveryFolder/alloy_SC.als) to formally model the system's behavior, verify the contract execution flow, and ensure proper constraints.

---

## 👥 Authors

Project developed by:
* **Rodari Simone**
* **Bogdanovic Stefan**
* **Pignataro Gabriele**
