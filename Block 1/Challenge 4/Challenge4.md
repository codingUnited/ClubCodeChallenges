## 🗓️ Coding Club Challenge Series
## 🟦 Challenge 4: Twilio Messaging App
## ⏳ Duration: 4 weeks
## 🎯 Goal: Build a simple app that sends text messages using the Twilio API.

----

# 🔧 What You’ll Do (Easy Mode Walkthrough)

1. Go to your GitHub repo in the CodingClub organization
    - If you don’t have one yet, complete Challenge 1 (Git/GitHub setup).
2. Inside your repo, create a new folder named:
```bash
  Challenge4-Twilio
```
3. Inside that folder, create a new file:
```bash
  send_sms.py
```
4. Set up Twilio
    - Go to [Twilio](https://www.twilio.com/) and create a free account.
    - Grab your Account SID, Auth Token, and a trial phone number from the [Twilio Console](https://www.twilio.com/console).
5. Install the Twilio library

Run in your terminal:
```bash
  pip install twilio
```

6. Add this starter code to ```send_sms.py```:
```python
from twilio.rest import Client

# Replace these with your actual credentials
account_sid = "your_account_sid"
auth_token = "your_auth_token"
client = Client(account_sid, auth_token)

message = client.messages.create(
    body="Hello from Coding Club Challenge 4!",
    from_="+1234567890",  # Your Twilio trial number
    to="+0987654321"      # Your own verified number
)

print("Message sent! SID:", message.sid)

```
7. Run your program:
```bash
python send_sms.py
```

✅ If successful, you should see Message sent! and receive a text on your phone.

8. Push your changes to GitHub
   
Make sure the Challenge4-Twilio folder and send_sms.py are committed and pushed.

----

## 📌 Submission Checklist (Easy Mode)

- ✅ Repo is public and still named challenge-yourName
- ✅ Folder Challenge4-Twilio exists in your repo
- ✅ File send_sms.py exists with Twilio starter code
- ✅ Program sends a text to your phone using Twilio
- ✅ Committed and pushed to GitHub

----

## 📝 Notes
- You’ll need to verify your personal phone number in the Twilio Console (trial accounts can only text approved numbers).
- Make sure you never push your real Auth Token to GitHub. Use a ```.env``` file or placeholders when committing.
- For advanced tiers (Medium/Hard/Leet), you’ll expand from here: add user input, build a GUI, or make a mobile app with a pass-through API.

📖 Twilio Docs: [https://www.twilio.com/docs/sms](https://www.twilio.com/docs/sms)

🚀 Python Quickstart: [https://www.twilio.com/docs/sms/quickstart/python](https://www.twilio.com/docs/sms/quickstart/python)
