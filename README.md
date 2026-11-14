# KunUZ Clone

Django asosida yaratilgan yangiliklar sayti. Unda yangiliklar, kategoriyalar va Django Admin orqali kontent boshqaruvi mavjud.

## Texnologiyalar

- Python 3.11+
- Django 5.2
- Pillow

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
python manage.py migrate
python manage.py runserver
```

Sayt: http://127.0.0.1:8000/

Admin foydalanuvchi yaratish:

```bash
python manage.py createsuperuser
```

## Xavfsizlik

Deploy qilishdan oldin `DJANGO_SECRET_KEY`, `DJANGO_DEBUG=False` va `DJANGO_ALLOWED_HOSTS` muhit o'zgaruvchilarini sozlang. Haqiqiy maxfiy kalitni repozitoriyga joylamang. Avvalgi commitda ochiq turgan kalitni ham almashtiring.

## Muallif

Umidjon Abdullayev — https://github.com/umidjon3455
