# 🤖 AI B2B Lead Generation Automation

An intelligent lead generation workflow built using **n8n** that automatically discovers potential business leads, extracts company information using AI, removes duplicates, validates the data, and stores qualified leads in Google Sheets.

This workflow eliminates manual lead research by combining AI-powered web search, content analysis, and workflow automation.

---

# 📌 Project Overview

This automation is designed for agencies, freelancers, startups, and sales teams that require a continuous flow of qualified B2B leads.

The workflow automatically searches for companies within predefined target industries, extracts structured business information using Google Gemini AI, filters duplicate entries, validates lead quality, and saves the final dataset into Google Sheets.

---

# 🚀 Workflow Overview

```
Schedule Trigger
      │
      ▼
Define Target Audience
      │
      ▼
Generate Search Queries
      │
      ▼
Search Companies (Tavily AI)
      │
      ▼
Split Search Results
      │
      ▼
Check Existing Leads
      │
      ▼
Visit Company Website
      │
      ▼
Extract Website Content
      │
      ▼
Analyze with Gemini AI
      │
      ▼
Parse Structured Data
      │
      ▼
Format Lead
      │
      ▼
Validate Lead
      │
      ▼
Save to Google Sheets
```

---

# ✨ Features

## 🔍 AI-Powered Company Discovery

- Automatic company search
- Industry-specific lead generation
- AI-powered web search using Tavily

---

## 🌐 Website Analysis

- Visit company websites
- Extract website content
- Identify services and business information

---

## 🧠 AI Data Extraction

Google Gemini automatically extracts:

- Company Name
- Website
- LinkedIn Profile
- Business Location
- Industry
- Contact Email
- Decision Maker
- Company Description

---

## 📊 Lead Validation

- Duplicate detection
- Remove incomplete records
- Validate contact information
- Quality filtering

---

## 📄 Google Sheets Integration

Automatically stores qualified leads including:

| Field |
|--------|
| Company Name |
| Company Website |
| Company LinkedIn |
| Company Location |
| Contact Email |
| Industry |
| Decision Maker |
| Date Added |

---

# ⚙ Workflow Components

## 1. Schedule Trigger

Runs automatically at a predefined time (e.g., daily at 9:00 AM IST).

---

## 2. Target Audience Generator

Defines industries and business sectors to search.

Example:

- Healthcare
- Medical Billing
- SaaS
- E-Commerce
- Manufacturing
- Logistics
- IT Services
- Finance

---

## 3. Search Query Generator

Creates optimized search queries dynamically.

Example:

```
Top Healthcare Companies in Texas

Medical Billing Companies USA

Software Companies in California
```

---

## 4. Tavily Search

Uses Tavily AI Search API to discover businesses from the web.

Returns:

- Website
- Description
- Search snippet
- URLs

---

## 5. Website Scraper

Visits each company website.

Extracts:

- Contact Page
- About Us
- Services
- Email
- Address

---

## 6. Google Gemini AI

Processes website content and converts unstructured text into structured JSON.

Example Output

```json
{
  "companyName": "",
  "website": "",
  "linkedin": "",
  "email": "",
  "location": "",
  "sector": "",
  "decisionMaker": ""
}
```

---

## 7. Data Formatter

Formats AI output into a consistent schema.

---

## 8. Lead Validation

Checks:

- Missing fields
- Invalid emails
- Duplicate companies
- Existing records

---

## 9. Google Sheets Storage

Stores validated leads automatically.

---

# 🛠 Technologies Used

### Automation

- n8n

### AI

- Google Gemini API

### Search

- Tavily AI Search

### Storage

- Google Sheets

### APIs

- HTTP Request Nodes
- Google Sheets API

### Data Processing

- JavaScript
- JSON

---

# 📂 Workflow Structure

```
AI-B2B-Lead-Generator/

│
├── Trigger
├── Define Target Audience
├── Generate Search Query
├── Tavily Search
├── Split Results
├── Duplicate Checker
├── Website Scraper
├── Website Cleaner
├── Gemini AI
├── Parse JSON
├── Format Data
├── Lead Validation
├── Google Sheets
└── README.md
```

---

# 📈 Use Cases

Perfect for:

- AI Automation Agencies
- Digital Marketing Agencies
- Sales Teams
- Freelancers
- B2B Companies
- Recruitment Firms
- Lead Generation Agencies
- Startup Founders

---

# 🎯 Benefits

✅ Fully Automated

✅ AI-Powered Lead Research

✅ No Manual Data Entry

✅ Duplicate Prevention

✅ Structured Business Information

✅ Daily Lead Generation

✅ Google Sheets Integration

✅ Scalable Workflow


# 🔮 Future Improvements

- LinkedIn Company Scraping
- Apollo.io Integration
- Hunter.io Email Verification
- Clearbit Enrichment
- CRM Integration (HubSpot, Salesforce)
- Email Outreach Automation
- WhatsApp Notifications
- AI Lead Scoring
- Multi-language Company Search
- CSV/Excel Export
- Slack Notifications



# 📸 Workflow Screenshot

<img width="1458" height="360" alt="image" src="https://github.com/user-attachments/assets/7c5078d1-3a48-4847-af8b-7e9a20db80d7" />


# ⚙ Installation

## Requirements

- n8n
- Google Gemini API Key
- Tavily API Key
- Google Sheets Credentials



## Setup

1. Clone this repository

```bash
git clone https://github.com/yourusername/lead-generator.git
```

2. Import the workflow into n8n.

3. Configure the following credentials:

- Tavily API
- Google Gemini API
- Google Sheets OAuth2

4. Update the target industries.

5. Activate the workflow.



# 📊 Output Example

| Company | Website | LinkedIn | Email | Industry | Location |
|----------|----------|----------|--------|----------|----------|
| ABC Corp | abc.com | linkedin.com/company/abc | info@abc.com | Healthcare | USA |



# 👨‍💻 Developer

**Varun Kumar**

AI Automation Developer | Full Stack Developer | Workflow Automation Specialist

### Skills

- n8n Automation
- AI Agents
- Google Gemini
- OpenAI
- Workflow Automation
- Lead Generation Systems
- Web Scraping
- API Integrations

### Connect

**GitHub**

https://github.com/Varunkumar-03

**Portfolio**

https://varunkumar03.netlify.app/

**LinkedIn**

https://www.linkedin.com/in/varun-kumar-b8274a280/


# ⭐ Support

If you found this workflow useful, please give this repository a ⭐ on GitHub.


# 📄 License

This project is licensed under the MIT License.


## 💡 Why This Project?

Traditional lead generation is time-consuming and repetitive. This workflow automates the entire process—from discovering companies to extracting structured business information—saving hours of manual effort while improving data quality and consistency.


Made with ❤️ by **Varun Kumar**
