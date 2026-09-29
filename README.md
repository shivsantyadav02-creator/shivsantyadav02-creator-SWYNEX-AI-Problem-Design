# shivsantyadav02-creator-SWYNEX-AI-Problem-Design# 
- Task 1: AI Problem Design

## 1. Problem Statement & Title
**Project Title:** Customer Feedback Sentiment & Topic Categorization Engine  
**Objective:** Automatically classify customer feedback into sentiment categories (Positive, Neutral, Negative) and functional tags (Product Quality, Customer Support, Pricing, Delivery) to reduce manual sorting time and prioritize urgent customer issues.

---

## 2. Target User & Use Case
- **Target User:** Customer Support Leads and Operations Managers at e-commerce/SaaS companies.
- **Use Case:** A narrow text classification pipeline that automatically ingests unstructured customer feedback, assigns sentiment scores, and routes negative/urgent complaints to dedicated support reps.

---

## 3. Data Source
- **Dataset:** Small dataset consisting of ~500–1,000 anonymized e-commerce reviews and support ticket logs.
- **Attributes:** `Review_Text`, `Rating`, `Timestamp`, `Category`.

---

## 4. Constraints & Limitations
- **Dataset Size:** Small dataset limits training complex deep learning models from scratch; fine-tuning pre-trained models or using API-based solutions is required.
- **Latency & Compute:** Classification response time must be under 2 seconds per request on basic CPU infrastructure.
- **Privacy Constraints:** All user personal identifying information (PII) must be anonymized before ingestion.

---

## 5. Success Criteria & Evaluation Approach
- **Quantitative Metrics:**
  - Accuracy & F1-Score: Macro F1-Score >= 0.85 across classification categories.
  - Latency: Average latency <= 1.5 seconds.
- **Qualitative Metrics:**
  - Support team usability and reduction in manually flagged tickets by at least 40%.
