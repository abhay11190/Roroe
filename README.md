# SellerSmart Support Bot — Render deployment v5

1. Extract this ZIP and upload the files in this folder to the ROOT of your GitHub repository (not inside another nested folder).
2. In Render, set Build Command: `pip install -r requirements.txt`
3. Set Start Command: `python sellersmart.py`
4. In Render Environment, set `BOT_TOKEN` to the NEW token from BotFather. Never paste the token into code, GitHub, or chat.
5. Set `PYTHON_VERSION` to `3.11.11` in Render Environment, then deploy latest commit.

This version increases Telegram HTTP connection/read timeouts and retries bootstrap polling. A persistent Render-to-Telegram network outage cannot be repaired by Python code alone.

Required bot permissions in the group: Add New Admins, Ban Users, Restrict Members, Pin Messages. Enable chat-member updates by keeping the bot as admin.
