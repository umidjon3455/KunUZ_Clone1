# KunUZ Clone

Django asosida yaratilgan yangiliklar sayti. Unda yangiliklar, kategoriyalar va Django Admin orqali kontent boshqaruvi mavjud.

## Texnologiyalar

- Python 3.11+
- Django 5.2
- Pillow
- python-dotenv

## O'rnatish

```bash
git clone https://github.com/umidjon3455/KunUZ_Clone1.git
cd KunUZ_Clone1
python -m venv .venv
```

Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Kutubxonalarni o'rnating:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

Muhit faylini yarating:

```powershell
Copy-Item .env.example .env
```

```bash
python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
```

Yangi kalitni `.env` faylidagi `DJANGO_SECRET_KEY` qiymatiga yozing. Lokal ishlash uchun `DJANGO_DEBUG=True` bo'lishi mumkin. Deploy vaqtida `DJANGO_DEBUG=False` va `DJANGO_ALLOWED_HOSTS` ni domeningizga moslang. `.env` faylini GitHub'ga yubormang.

Bazani tayyorlang va serverni ishga tushiring:

```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Sayt: http://127.0.0.1:8000/

Admin: http://127.0.0.1:8000/admin/

## Xavfsizlik

Oldingi commitlarda oshkor bo'lgan maxfiy kalitni qayta ishlatmang. Yangi kalit yarating va hostingdagi maxfiy sozlamalarni yangilang.

## Muallif

Umidjon Abdullayev — https://github.com/umidjon3455
