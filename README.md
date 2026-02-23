# Tanzeania S. | AWS Cloud & Generative AI Portfolio
> Professional portfolio showcasing technical skills and innovative solutions developed during the AWS re/Start program.

---

## 🤖 Artificial Intelligence Exploration

### Project: AI-Powered Academic Co-Pilot
**Goal:** Providing 24/7 Socratic tutoring for nontraditional students to bridge the gap in academic support.

#### 📍 Project Discovery & Scenario
To develop a high impact AI solution, I identified the following core needs and opportunities:

* **1. Who is the customer?** College students who require tutoring services outside of traditional business hours (9:00 AM – 5:00 PM).
* **2. Who is affected?** * **Students:** Full-time nontraditional learners with families, long work hours, and external commitments.  
    * **Faculty:** Professors aiming to provide 24/7 assistance without increasing their personal workload.  
    * **Institutions:** Schools looking to increase student retention and lower dropout rates through better support.
* **3. The Problem & Opportunity** Traditional tutoring and peer groups are often restricted to M-F business hours. This excludes the "after hours" learner. This project launches an on-demand, cost effective academic tool more accessible than a physical campus center.
* **4. The Solution: AI-Powered Academic Co-Pilot** A multi-modal interface featuring:
    * **Math Tutor (OCR):** Guided problem solving using Optical Character Recognition.
    * **Interactive Essay Architect:** Real time grammatical and structural feedback.
    * **Voice-Enabled "Rubber Ducking":** Audio based concept strengthening for students on the go.
* **5. Value Proposition** Provides immediate support during late night study sessions, preventing student frustration and reducing the likelihood of academic burnout.
* **6. Technical Workflow** The Co-Pilot utilizes **Contextual Awareness** (processing specific course materials) and **Socratic Scaffolding**. Instead of providing direct answers, it guides students through the logic. If a student remains stuck, the system automatically flags the concept for review during official professor office hours.

---

## 🏗️ Proposed Technical Architecture

To bring the **AI Academic Co-Pilot** to life, I have mapped the features to the following AWS Cloud ecosystem:

| Feature | AWS Service | Purpose |
| :--- | :--- | :--- |
| **Brain & Logic** | **Amazon Bedrock** | Orchestrates Large Language Models (LLMs) like Claude or Llama to power the Socratic Tutor logic. |
| **Math OCR** | **Amazon Textract** | Extracts handwritten equations from student uploaded photos with high accuracy. |
| **Voice Interface** | **Amazon Polly & Transcribe** | Converts student speech to text (Rubber Ducking) and reads AI hints back to the student. |
| **Contextual Memory** | **Amazon Bedrock Knowledge Bases** | Connects the AI to specific course syllabi and PDFs using RAG (Retrieval Augmented Generation). |
| **Integrity Checks** | **Amazon Bedrock Guardrails** | Ensures the AI refuses to provide direct answers and remains within academic safety boundaries. |

### 🔄 The "Socratic" Data Flow
1. **Input:** Student uploads a problem (Image/Text/Voice).
2. **Analysis:** **Amazon Textract** or **Transcribe** converts the input to raw text.
3. **Reasoning:** **Amazon Bedrock** compares the input against "Knowledge Bases" (the syllabus).
4. **Scaffolding:** The LLM generates a guiding question rather than an answer.
5. **Output:** The student receives a hint via the **Multi-modal Interface**.
