# استفاده از پایتون نسخه 3.11
FROM python:3.11-slim

# تنظیم دایرکتوری کاری
WORKDIR /app

# کپی فایل‌های پروژه به داخل کانتینر
COPY . /app

# نصب نیازمندی‌ها
RUN pip install --upgrade pip && pip install django djangorestframework

# باز کردن پورت 8000
EXPOSE 8000

# دستور اجرا هنگام بالا اومدن کانتینر
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
