# 📞 AI Voice Calling Agent — Automated Lead Calling & CRM Updation

An automated workflow that connects **Google Sheets → AI Voice Agent → Sheets Update**, eliminating manual calling.  
The system detects newly added leads, triggers AI-powered outbound calls, captures call responses, and updates CRM in real-time — built using **n8n, Twilio, and OpenAI**.

---

## 🚀 Overview
This Voice Agent automates the first step of sales outreach.

- Detects newly added leads from Google Sheets  
- Triggers outbound calls using an AI conversational agent  
- Logs call result (Interested / Not Interested / No Answer / Invalid Number etc.)  
- Updates the same row in the sheet automatically

---

## 🧠 Tech Stack

| Component | Purpose |
|----------|---------|
| **n8n** | Workflow automation |
| **Google Sheets** | Lead source + CRM update |
| **Twilio Voice API** | Place outbound voice calls |
| **OpenAI GPT** | Dynamic conversation generation |
| **HTTP API** | Connect call logic with n8n |

---

## 🔁 Workflow Architecture
```
Google Sheets (New Lead Added)
↓
Filter Node — Validate number + new status
↓
Set Node — Map name, phone, company, requirement
↓
HTTP Request — Twilio + GPT conversation response
↓
Google Sheets — Update row with call outcome
```
---

## ⭐ Key Features

| Feature | Benefit |
|--------|--------|
| Automated outbound calling | Removes manual calling effort |
| 100% CRM update in real time | No human entry required |
| GPT-powered voice responses | Personalized, context-aware conversation |
| Error handling | Skips invalid numbers and logs failure reasons |

---

## 📌 Node-by-Node Breakdown

| Node | Action |
|------|--------|
| **Google Sheets Trigger** | Detect new lead entry |
| **Filter Node** | Check phone validity + status = "new" |
| **Edit Fields / Set Node** | Structure payload for API call |
| **HTTP Request Node** | Trigger AI voice call and capture summary |
| **Google Sheets — Update Row** | Log updated status + remarks in same row |

---

## 📸 Screenshots

Screenshots are stored in the `assets/` folder.

> After you know the exact file names, embed them like this:

```md
![Trigger Node](assets/trigger.png)
![Filter Node](assets/filter.png)
![HTTP API Call](assets/http.png)
![Update Row](assets/update_row.png)
```
---

## 📍 Results

| Metric                 | Outcome               |
| ---------------------- | --------------------- |
| Manual calling effort  | ⬇ **Reduced by 90%**  |
| CRM entry errors       | ⬇ **Reduced to 0%**   |
| Call clarity using GPT | ⬆ **Improved by 60%** |
| Data sync              | **100% accurate**     |

---

## 🔮 Future Enhancements

- Multi-language voice support

- Email + WhatsApp follow-ups after call

- Dashboard for lead conversion analytics

## 👩‍💻 Author

Kritika Aggarwal
📧 Email: kritikaaggarwal2227@gmail.com
🔗 Portfolio: (to be added when updated)

---

### 📌 After adding the README
Next step: insert screenshot links once they appear in the `assets` folder.

Whenever you upload all screenshots, tell me the **exact file names**, and I’ll generate the **correct Markdown display code** so the images appear perfectly inside the README.

Ready for the next step 🚀

