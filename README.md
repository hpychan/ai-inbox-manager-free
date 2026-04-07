# AI Inbox Manager - Free Version

Reduce email noise by 90% — automatically.

Only see what matters. Ignore the rest.

This workflow scans your inbox and sends a clean summary of important emails to Telegram.
No coding required. Setup takes ~3-5 minutes.

## Quick Start (2 minutes)

1. Import `PA_Gmail_Triage_FREE.json` into n8n.
2. Connect credentials:
   - Gmail
   - Gemini (AI)
   - Telegram
   
👉 [Follow the Quick Setup section below](#quick-setup-5-minutes)

3. Set your Telegram `chatId`.
4. Click **"Execute workflow" on the Manual Trigger node** to test.

You should receive a message in Telegram.

## Expected Output

You will receive a Telegram message like:

📬 AI Inbox Summary  
🔥 1 Important Email  
• Subject: Login alert  
• Action: Review immediately

👉 Example:
![Telegram example output](free-telegram-example.png)

If you see this message, your setup is working correctly.

## What you'll get

- Detects important emails automatically  
- Sends a clean summary to Telegram  
- No auto-delete or risky actions (safe to try)

## Important

- The workflow runs manually in the free version.
- `Gmail Trigger` is disabled by default for safety.
- Only enable it after testing successfully.

## Troubleshooting

**No Telegram message?**
- Check your `chatId`.
- Make sure your bot has received at least 1 message from you.

**No emails found?**
- Make sure you have unread emails.
- Check Gmail credentials.

## Quick Setup (5 minutes)

1. **Gmail (OAuth)**
   - Click `Add credential` in n8n.
   - Select Gmail.
   - Login with your account.

   ✔ Connected

2. **Gemini (AI)**
   - Go to [https://aistudio.google.com](https://aistudio.google.com).
   - Create API key.
   - Paste into n8n credential.

   ✔ Connected

3. **Telegram Bot**
   - Open Telegram.
   - Search: `BotFather`.
   - Run: `/newbot`.
   - Copy bot token.
   - Message your bot once.

   ✔ Connected

4. **Get Chat ID**
   - Open in browser:
     `https://api.telegram.org/bot<TOKEN>/getUpdates`
   - Look for:
     `"chat": { "id": XXXXX }`
   
   Use this number as your `chatId`.

## Upgrade (optional)

Unlock automation and save more time:

- Runs automatically every hour  
- Smarter prioritization  
- Task extraction (Google Tasks)  
- Cleaner, structured summaries  

Designed for daily use.
