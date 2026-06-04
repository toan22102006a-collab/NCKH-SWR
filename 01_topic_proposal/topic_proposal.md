# Topic Proposal

## 1. Group Information

- Class: SE2037
- Group: 03
- Leader: Nguyen Trong Toan
- Members: Huynh Viet Phat, Pham Trong Nghia, Vu Tran Phuc Khang, Phan Bao Duy

## 2. Proposed Title

**English title: Requirements Engineering for an AI-based Student Early Warning System.**

**Vietnamese title: Thiết kế yêu cầu kỹ thuật cho hệ thống cảnh báo sớm dành cho học sinh dựa trên trí tuệ nhân tạo.**

## 3. Application Domain

- Application domain: Student Support/ Learning Management/ Smart Education.

## 4. Problem Statement

- Limitations of Current Academic Warning Systems: Traditional Academic Information Systems (AIS) operate reactively and often generate performance data only at the end of a semester when student attrition or course failure is already irreversible. Consequently, stakeholders cannot intervene timely when a student's attendance drops or learning is interrupted.

- The Resource & Recommendation Issues: While massive amounts of educational materials exist, current platforms lack the capability to dynamically map specific student vulnerabilities to precise remedial resources to help struggling students without a clear, personalized recovery roadmap.

- The Requirements Engineering (RE) Challenge (The Core): From a system design perspective, a critical challenge lies in the paradigm shift from traditional code-defined systems to data-driven AI behaviors. Traditional RE frameworks are built to capture deterministic requirements implemented via hard-coded logic. However, integrating AI components introduces significant non-deterministic errors, such as data bias in predictive models (Random Forest) and hallucinations in generative systems (RAG/LLM). Moreover, engineering a reliable system requires continuous collection of training data and stakeholder feedback. This creates a major methodological gap: current RE frameworks lack the formal processes to systematically translate vague stakeholder expectations, domain feedback, and raw academic data into precise technical workflows, mitigation constraints, and functional specifications for AI components.

## 5. Motivation

- Practical Motivation:
  - Academic failure and dropouts cause big problems for both schools and students. For schools, high dropout rates damage their reputation and reduce their financial income. For students, failing a course wastes their time and money, and easily leads to serious mental health issues like stress and depression. By using AI to warn students early, schools can help them in time and reduce these negative impacts before it is too late.
- Engineering Motivation:
  - Building an AI educational system without a clear Requirements Engineering (RE) process is very risky. Without it, engineers might build a flawed AI that gives wrong warnings (causing unnecessary panic for students) or creates incorrect study plans (harming how students learn). Therefore, designing a proper RE framework is the key to success. It ensures the AI system is safe, accurate, and works exactly how teachers and students expect.

## 6. Target Users

- Target Users:

1. School managers/ Academic Administrators:

- Role: Monitor overall institutional performance and ensure system data privacy compliance.
- AI Interaction: Rely on macro-level analytics from the predictive model to manage school resources.

2. Teachers/ Academic Advisors:

- Role: Review AI-generated warnings and study plans before they reach students.
- AI Interaction: Provide professional feedback to correct AI errors (hallucinations) and interpret model predictions through explainable interfaces.

3. Students:

- Role: The primary beneficiaries who receive early warnings and personalized remedial roadmaps.
- AI Interaction: Input academic data (grades, attendance) and provide user feedback on the quality of recommended documents to help improve the system.

## 7. Proposed AI Model / Method

1. Random Forest: Used for predictive analytics to calculate student failure or dropout risks based on historical data.

2. Retrieval-Augmented Generation (RAG): Used to fetch precise, verified educational documents and school syllabus context.

3. Large Language Models (LLM): Used to generate personalized study plans based on the context provided by RAG.

## 8. System Features

1. Functional Requirements (FRs)

- FR1: Early Risk Detection: The system must analyze student data (grades, attendance) using Random Forest to trigger warnings as soon as risk thresholds are met.

- FR2: Human-in-the-Loop Verification: The system must allow academic advisors to review, edit, and approve AI-generated study plans before sending them to students (to fix AI hallucinations).

- FR3: Personalized Roadmap Generation: The system must use RAG/LLM to create specific, step-by-step study roadmaps tailored to each flagged student's weaknesses.

- FR4: Resource Recommendation: The system must automatically match and recommend relevant study materials from the school portal to the student.

- FR5: Feedback Collection: The system must collect ratings and text feedback from advisors and students to improve future AI training data.

2. Non-functional Requirements (NFRs)

- NFR1: Accuracy & Reliability: The predictive model must maintain high precision to avoid false alarms that cause student panic.

- NFR2: Faithfulness (Anti-Hallucination): The LLM must strictly use data from the approved school syllabus (via RAG) to ensure zero incorrect information in study plans.

- NFR3: Data Privacy & Security: The system must protect student identity and sensitive academic records according to data safety regulations.

## 9. Expected Contribution

1. Practical & Educational Contributions:

- Proactive Support: Reduces student failure and dropout rates by enabling timely, data-backed interventions.

- Enhanced Management: Increases the efficiency of academic departments and helps advisors manage at-risk students with less manual effort.

2. Software Engineering Contributions:

- A Formal RE Framework: Provides a structured Requirements Engineering framework specifically designed for AI-driven academic systems, bridging the gap between vague stakeholder needs and technical AI specifications.

- Mitigation Guidelines: Establishes clear engineering requirements to systematically control data bias (in Random Forest) and eliminate hallucinations (in RAG/LLM) through human-in-the-loop workflows.

## 10. Evaluation Plan

1. Requirements Quality Evaluation (The Core Verification):

- Method: Use a panel of 3 Software Engineering experts to review the proposed RE framework.

- Criteria: Evaluate the requirement specifications based on Completeness, Consistency, and Verifiability using standard IEEE/ISO quality checklists.

2. AI Model Evaluation (Technical Metrics):

- Predictive Model (Random Forest): Evaluated using Accuracy, Precision, Recall, and F1-Score on historical student portals data.

- Generative Model (RAG/LLM): Evaluated using Faithfulness (no hallucinations) and Answer Relevance (matching the school syllabus).

3. Human & Operational Evaluation (Validation):

- Expert Review: 3 to 5 academic advisors will grade 50 AI-generated study plans to check their pedagogical usefulness and safety.

- User Survey: A survey sent to 100 students to measure user satisfaction and whether the recommended documents actually helped them improve.

## 11. Related Papers

| No  | Title                                                                                                                                                    | Year | Source                                | Link                                                                                                                           | Category             |
| :-- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | -------------------- |
| 1   | Ethical Imperatives and Challenges: Review of the Use of Machine Learning for Predictive Analytics in Higher Education                                   | 2024 | Digital Commons@Lindenwood University | https://digitalcommons.lindenwood.edu/cgi/viewcontent.cgi?article=1645&context=faculty-research-papers                         | Directly Related (1) |
| 2   | Predicting Student Academic Performance in Higher Education Using Data Mining: A Systematic Review                                                       | 2022 | Wiley Online Library                  | https://onlinelibrary.wiley.com/doi/full/10.1155/2022/8924028                                                                  | Directly Related (2) |
| 3   | Development of a Framework for Predicting Students' Academic Performance in STEM Education using Machine Learning Methods                                | 2024 | ResearchGate                          | https://www.researchgate.net/profile/Assyl-Tuimebayev/publication/378141724_Development_of_a_Framework_for_Predicting_Students | AI Method (1)        |
| 4   | Investigating the Performance of Retrieval-Augmented Generation and Domain-Specific Fine-Tuning for the Development of AI-Driven Knowledge-Based Systems | 2024 | MDPI                                  | https://www.mdpi.com/2504-4990/7/1/15                                                                                          | AI Method (2)        |
