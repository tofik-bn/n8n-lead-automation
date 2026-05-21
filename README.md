# AI Lead Response System

An automated AI agent that responds to website contact form submissions **within 5 minutes** – sending a warm, personalized email from the business owner and notifying them via SMS.

Built as a no‑code/low‑code workflow in **n8n** (cloud free tier). Fully reusable – can be imported for any local business in under 10 minutes.

## How it works

1. **Trigger:** Webhook receives lead data (name, email, message) from a website contact form.
2. **AI Understanding:** Groq API (free, fast) reads the message and generates a professional, human‑sounding email reply.
3. **Email Response:** Resend API sends the AI‑generated email to the lead.
4. **SMS Notification:** Twilio sends a summary to the business owner (API ready – trial limitations may apply for international SMS).
5. **Logging:** Every lead is automatically logged to Google Sheets with timestamp, AI response, and response time.

## Tech stack

- **n8n** – workflow orchestration (exported JSON)
- **Groq** – free LLM (Llama 3.1 8B)
- **Resend** – free email API (3000 emails/month)
- **Twilio** – SMS notification (trial account)
- **Google Sheets** – logging

## How to use

1. Import the `ai-lead-response-system.json` into your n8n instance.
2. Add your own API keys for Groq, Resend, Twilio, and Google Sheets.
3. Update the webhook URL in your website’s contact form (POST request with JSON body).
4. Test with a sample lead – the AI will reply instantly.

## Skills demonstrated

- API integration (REST, authentication, webhooks)
- AI prompt engineering
- Data transformation (ETL)
- Email automation
- SMS automation
- Google Sheets logging
- Low‑code workflow design (n8n)

## Author

Your Name – https://www.linkedin.com/in/taoufik-bani-761a6836a/

## License

MIT
