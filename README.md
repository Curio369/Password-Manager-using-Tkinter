# 🔐 MyPass — Password Manager

> A simple, local-first desktop password manager built with Python and Tkinter. Generate strong passwords, save credentials securely in a JSON file, and look them up instantly — all from a clean GUI.

---

## 📸 Preview

![MyPass Screenshot](img/sample.png)

---

## ✨ Features

- 🔑 **Password Generator** — Creates strong random passwords (letters + symbols + numbers) and auto-copies to clipboard
- 💾 **Save Credentials** — Stores website, email/username, and password in a local `data.json` file
- 🔍 **Search Passwords** — Instantly look up saved credentials by website name
- 📋 **Clipboard Support** — Generated passwords are automatically copied via `pyperclip`

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.8+ | Core language |
| Tkinter | GUI framework |
| JSON | Local credential storage |
| pyperclip | Clipboard integration |

---

## ⚙️ Configuration

> [!IMPORTANT]
> Before running the app, set your default email in `main.py` on **line 103**:
> ```python
> email_entry.insert(0, "your@email.com")  # Replace with your email
> ```
> This email will be pre-filled in the Email/Username field every time you launch the app.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/mypass.git
cd mypass
```

### 2. Install dependencies

Using **Poetry** (recommended):
```bash
poetry install
poetry run python main.py
```

Or using **pip**:
```bash
pip install pyperclip
python main.py
```

---

## 📁 Project Structure

```
mypass/
├── main.py          # Main application
├── logo.png         # App logo
├── data.json        # Auto-generated credential store (gitignored)
├── img/
│   └── sampleimg.png
├── pyproject.toml
└── poetry.lock
```

> ⚠️ **Note:** `data.json` is created automatically on first save. Make sure to add it to your `.gitignore` to keep your credentials safe.

---

## 🔒 Security Note

Passwords are stored in **plain text** in `data.json` locally on your machine. This project is intended for learning purposes. For production use, consider encrypting the JSON file or using a dedicated secrets manager.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
