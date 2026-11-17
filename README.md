# KunUZ Clone

Django asosida yaratilgan yangiliklar sayti. Unda yangiliklar, kategoriyalar va Django Admin orqali kontent boshqaruvi mavjud.

## Texnologiyalar

- Python 3.11+
- Django 5.2
- Pillow
- python-dotenv

## O'rnatish

Repozitoriyani yuklab oling va loyiha papkasiga kiring:

```bash
git clone https://github.com/umidjon3455/KunUZ_Clone1.git
cd KunUZ_Clone1
python -m venv .venv
```

Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
Copy-Item .env.example .env
```

macOS/Linux:

```bash
source .venv/bin/activate
cp .env.example .env
```

**Muhim:** `.env` faylini oching va `DJANGO_SECRET_KEY` qiymatini yangi, tasodifiy maxfiy kalitga almashtiring. Kalit yaratish:

```bash
python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
```

Kutubxonalarni o'rnating va serverni ishga tushiring:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Sayt: http://127.0.0.1:8000/

Admin foydalanuvchi yaratish:

```bash
python manage.py createsuperuser
```

## Muhit o'zgaruvchilari

- `DJANGO_SECRET_KEY` — maxfiy kalit; repozitoriyga joylamang.
- `DJANGO_DEBUG=True` — faqat lokal ishlab chiqish uchun. Production muhitida `False` qiling.
- `DJANGO_ALLOWED_HOSTS` — domenlar ro'yxati, vergul bilan ajratiladi.

## Xavfsizlik

Haqiqiy `.env` fayli Git'ga qo'shilmaydi. Avvalgi commitlarda ochiq bo'lgan maxfiy kalitlarni yangi kalit bilan almashtiring.

## Muallif

Umidjon Abdullayev — https://github.com/umidjon3455
