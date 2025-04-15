## 📘 **README.md**

```markdown
# 🤖 Gemini AI Telegram Bot

A powerful, interactive Telegram bot that leverages Google's Gemini API to provide:
- Text-based AI responses
- Image generation
- Voice message transcription and replies
- User access control (admin-restricted)

---

## 🚀 Features

- 🧠 Chat with Gemini 1.5 Pro
- 🎨 Generate images using Gemini 2.0 Flash
- 🎤 Voice-to-text transcription and AI responses
- 🔒 Access control (admin-only and authorized users)
- 🔧 Command handlers for management
- 📂 Logs all activity to `telegram_bot.log`

---

## 🛠️ Requirements

- Python 3.9+
- Telegram Bot Token
- Google Gemini API Key
- Admin Telegram User ID

---

## 📦 Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/gemini-telegram-bot.git
cd gemini-telegram-bot
```

2. **Install dependencies:**

```bash
pip install -r requirements.txt
```

3. **Set environment variables:**

```bash
export TELEGRAM_TOKEN="your-telegram-bot-token"
export GEMINI_API_KEY="your-google-gemini-api-key"
export ADMIN_USER_ID="your-telegram-user-id"
```

Optionally, use a `.env` file with [python-dotenv](https://pypi.org/project/python-dotenv/) for easier config.

---

## 🧑‍💻 Usage

```bash
python bot.py
```

The bot will start in long-polling mode.

---

## 💬 Commands

| Command        | Description                                      |
|----------------|--------------------------------------------------|
| `/start`       | Welcome message and usage instructions           |
| `/help`        | Help message with tips                          |
| `/image`       | Generate an image from a description             |
| `/whoami`      | Display your user ID and authorization status    |
| `/auth <id>`   | (Admin only) Authorize a user ID                 |
| `/revoke <id>` | (Admin only) Revoke access from a user ID        |
| `/users`       | (Admin only) List authorized users               |

---

## 🔐 Access Control

- Only users listed in `authorized_users.json` can interact with the bot.
- The admin can add or revoke users using `/auth` and `/revoke`.

---

## 🧪 Sample Usage

**Text Response:**
> User: "What's the capital of France?"
> Bot: "💬 You asked: 'What's the capital of France?' 🤖 Response: Paris is the capital of France 🇫🇷"

**Image Generation:**
> `/image a futuristic city skyline at sunset in cyberpunk style`

**Voice Message:**
> Send a voice clip — Bot will transcribe and respond intelligently.

---

## 🐛 Logging

- All logs are stored in `telegram_bot.log` for auditing and debugging.

---

## 📄 License

MIT License. Feel free to modify and share.

---

## 👤 Author

Developed by [@alwalid54321](https://t.me/alwalid54321)

```
