# Document QA System

این پروژه یک سامانه پرسش و پاسخ از روی فایل‌های Word است که با Django ساخته شده است.

کاربر می‌تواند فایل Word با فرمت `.docx` آپلود کند، سیستم متن فایل را استخراج می‌کند، سپس کاربر می‌تواند درباره همان فایل سؤال بپرسد و سیستم با کمک مدل هوش مصنوعی از طریق OpenRouter پاسخ تولید می‌کند.

---

## امکانات پروژه

- آپلود فایل Word با فرمت `.docx`
- استخراج خودکار متن از فایل Word
- ذخیره متن استخراج‌شده در دیتابیس
- پرسیدن سؤال درباره سند
- ارسال متن سند و سؤال به مدل هوش مصنوعی
- دریافت پاسخ از AI
- ذخیره تاریخچه سؤال و جواب
- مدیریت اسناد از طریق Django Admin
- ارائه API با Django REST Framework

---

## تکنولوژی‌های استفاده‌شده

- Python
- Django
- Django REST Framework
- SQLite
- python-docx
- LangChain
- OpenRouter API
- python-dotenv

---

## ساختار کلی پروژه

```text
Myprojects/
├── manage.py
├── .env
├── .env.example
├── README.md
├── requirements.txt
├── db.sqlite3
├── documents/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── serializers.py
│   ├── ai.py
│   ├── utils.py
│   └── admin.py
├── core/
│   ├── settings.py
│   └── urls.py
└── media/