
# LinkedIn Job Scraper with n8n Automation

This project automates the process of **scraping LinkedIn job postings**, extracting decision-maker information, verifying company details, and organizing the data in **Google Sheets** for further use. The workflow is built using **n8n** and integrates multiple APIs for a seamless data pipeline.

---

## 🚀 Features
- **Automated Job Scraping:** Collects job postings from LinkedIn via API requests.
- **Decision Maker Finder:** Uses third-party APIs to extract key company contacts.
- **Email Verification:** Verifies the extracted email addresses for accuracy.
- **Company Web Data Extraction:** Retrieves company websites and details.
- **Google Sheets Integration:** Stores all processed data in a structured format.
- **Conditional Routing:** Handles missing or invalid data gracefully using Switch nodes.
- **Lead Generation Integration:** Optionally connects with tools like Apollo.io or HeyReach for outreach campaigns.

---

## 🛠️ Tools & Technologies
- **n8n** – Workflow automation platform.
- **LinkedIn Job API** – For job scraping.
- **Google Sheets API** – For storing processed data.
- **Decision Maker Finder API** – To extract company decision-makers.
- **Email Verification API** – For validating emails.
- **Apollo.io / HeyReach API** – For lead generation and outreach campaigns.
- **HTTP Request Nodes** – For API calls.
- **Switch & Filter Nodes** – For conditional logic and error handling.

---

## ⚙️ Workflow Overview
1. **LinkedIn Job Scraping** – Extracts job postings using HTTP Request nodes.
2. **Decision Maker Finder** – Fetches key contacts for each company.
3. **Email Verification** – Validates email addresses using a verification API.
4. **Company Web Data Retrieval** – Extracts additional company details.
5. **Data Storage in Google Sheets** – Appends structured job and contact data.
6. **Lead Generation Integration** – Sends validated leads to outreach tools if configured.

---

## 📂 Project Structure
```
LinkedIn Job Scraper/
│-- Linkedin Job Scraper.json   # n8n workflow export file
│-- README.md                   # Project documentation
```

---

## 📋 Prerequisites
- **n8n Cloud or Self-Hosted Instance**
- **Google Sheets API Credentials**
- **LinkedIn API Access (if required)**
- **Decision Maker Finder API Key**
- **Email Verification API Key**
- **Apollo.io / HeyReach API Key (optional)**

---

## ▶️ How to Use
1. Import the `Linkedin Job Scraper.json` file into your n8n instance.
2. Set up the required **API credentials** in n8n:
   - Google Sheets
   - LinkedIn (if applicable)
   - Decision Maker Finder
   - Email Verification
   - Apollo.io / HeyReach (optional)
3. Run the workflow to start scraping and processing data.
4. View the processed job leads in **Google Sheets** or send them to outreach tools.

---

## 📈 Future Improvements
- Add error logging for failed API calls.
- Schedule workflows for automatic daily runs.
- Enhance data enrichment with additional APIs.

---

## 🤝 Contributing
Feel free to fork this repo, create issues, or submit pull requests to improve the project.

---

## 📜 License
This project is open-source under the MIT License.
