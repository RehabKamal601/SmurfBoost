
---

````markdown
# SmurfBoost – Backend

🎮 SmurfBoost is a powerful backend service built with **Django** designed to support advanced features like user authentication, OAuth login, user management, and more – ideal for game-related or performance-boosting platforms.

## 🚀 Features

- 🔐 Google OAuth2 Authentication
- 👥 Custom User Model
- 🌐 API Routing with DRF
- 📁 Environment-based settings
- 🧪 Testing with Pytest
- 📦 Docker support for local dev
- 🌍 i18n / l10n support (EN, FR, PT)

---

## 🛠️ Tech Stack

- Python 3.11+
- Django 4+
- Django REST Framework
- Celery (background tasks)
- PostgreSQL
- Docker & Docker Compose
- Redis (for Celery broker)
- GitHub Actions (CI/CD-ready)

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/RehabKamal601/SmurfBoost.git
cd SmurfBoost/Backend
````

### 2. Create and activate virtual environment

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r smurfboost/requirements/local.txt
```

### 4. Set up `.env` file

Copy and configure environment variables:

```bash
cp smurfboost/env.example .env
```

Edit `.env` and add:

```env
DJANGO_SECRET_KEY=your-secret
DEBUG=True
ALLOWED_HOSTS=127.0.0.1,localhost

# Google OAuth
SOCIAL_AUTH_GOOGLE_CLIENT_ID=your-client-id
SOCIAL_AUTH_GOOGLE_SECRET=your-client-secret
```

### 5. Run development server

```bash
python smurfboost/manage.py migrate
python smurfboost/manage.py runserver
```

---

## 🧪 Running Tests

```bash
pytest
```

---

## 📁 Project Structure

```
Backend/
│
├── smurfboost/
│   ├── config/         # Django settings (base, local, prod)
│   ├── users/          # Custom user model & APIs
│   ├── templates/      # Default HTML templates
│   ├── static/         # Static files (CSS, JS, images)
│   └── locale/         # Language translations
│
├── .env                # Local environment variables (excluded from git)
├── requirements/       # Dependencies (base, local, prod)
└── docker-compose.*    # Docker configs
```

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](smurfboost/LICENSE) file for details.

---

## 🙋 Author

**Rehab Kamal** – [GitHub Profile](https://github.com/RehabKamal601)

---

> 💡 *Tip: Always keep your `.env` secrets out of source control.*

```

---

هل تحبي أجهزه كملف جاهز `.md` أو PDF أو أضيف فيه مزيد من الأقسام مثل API endpoints أو روابط التوثيق؟
```
