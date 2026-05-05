# SEO_AUDIT_AI_AUTOMATION

# 🚀 AI SEO Audit Tool (n8n)

An automated SEO analysis tool built using **n8n**, capable of analyzing live websites and generating actionable SEO insights using rule-based logic and AI.

---

## 📌 Project Overview

This project allows users to input a website URL and receive a detailed SEO report including:

* Title & Meta Description analysis
* Heading structure (H1, H2)
* Internal link count
* Image ALT tag analysis
* Word count evaluation
* SEO score calculation
* AI-powered recommendations

---

## ⚙️ Workflow Architecture

Webhook → HTTP Request → Code → OpenAI → Google Sheets → Respond to Webhook

---

## 🛠️ Tech Stack

* n8n (Workflow Automation)
* JavaScript (Code Node)
* OpenAI API (AI Insights)
* Google Sheets API (Data Storage)

---

## 🔄 How It Works

1. User sends a request with a website URL
2. Webhook receives the request
3. HTTP Request node fetches HTML content
4. Code node extracts SEO elements
5. SEO score is calculated based on rules
6. OpenAI generates insights and suggestions
7. Data is stored in Google Sheets
8. Final report is returned to the user

---

## 🧪 Example Input

```json
{
  "url": "https://kct.ac.in/"
}
```

---

## 📊 Example Output

```json
{
  "url": "https://kct.ac.in/",
  "seo_score": 85,
  "issues": "Images missing alt tags",
  "word_count": 1200,
  "internal_links": 25,
  "ai_report": "The website has a good structure but can improve accessibility..."
}
```

---

## 📈 Features

* Real-time website SEO analysis
* Automated SEO scoring system
* AI-generated optimization suggestions
* Google Sheets integration for tracking
* API-based workflow using Webhook

---

## 🚀 How to Run

1. Clone this repository
2. Import workflow into n8n
3. Configure:

   * Webhook node
   * OpenAI API key
   * Google Sheets credentials
4. Execute workflow
5. Test using browser or Postman:

```
http://localhost:5678/webhook-test/seo-audit?url=https://example.com
```

---

## 📂 Project Structure

* n8n workflow JSON (exported file)
* README.md
* Screenshots (optional)

---

## 💼 Use Cases

* SEO analysis automation
* Digital marketing reporting
* Website audit tools
* Learning AI + automation workflows

---

## 📌 Future Improvements

* Add React frontend UI
* Improve SEO scoring algorithm
* Add keyword analysis module
* Integrate page speed insights API

---

## 🙌 Author

Santhi S

---

## ⭐ If you like this project

Give it a star ⭐ and share it!
