# VodiWalker Professional 22

نسخه Premium Control Center با Subscription Center جدید، Appearance Studio حرفه‌ای، رنگ‌ها و فونت‌های بیشتر و مدیریت کارت‌محور اینباندها.

## قابلیت‌های مهم
- Subscription Portal حرفه‌ای با مصرف زنده، QR، کپی/دریافت و پروفایل اتصال
- Appearance Studio: فونت، اندازه متن، Dark/Light/System، ۱۰ رنگ، تراکم، گوشه‌ها، Glow، Animation و Sidebar
- Inbound Board کارت‌محور با وضعیت، پروتکل، شبکه، امنیت، پورت، مصرف، اتصال، IP و انقضا
- Railway Auto Network و پشتیبانی از متغیرهای Railway
- Telegram Sales/Management Bot
- Login با username

Railway متغیرهای `RAILWAY_PUBLIC_DOMAIN`، `RAILWAY_TCP_PROXY_DOMAIN`، `RAILWAY_TCP_PROXY_PORT` و `RAILWAY_TCP_APPLICATION_PORT` را فراهم می‌کند و پنل از آن‌ها برای شبکه عمومی استفاده می‌کند.

اجرای Railway:
`uvicorn main:app --host 0.0.0.0 --port ${PORT:-8000}`

### Message Center
پنل دارای بخش «پیام‌ها» است که خطاهای Backend و خطاهای Frontend مرورگر را جمع‌آوری می‌کند. مسیرهای مدیریتی مرتبط:
- `GET /api/errors`
- `POST /api/errors/client`
- `POST /api/errors/clear`

برای Railway، healthcheck را روی `/health` قرار دهید. Railway در زمان healthcheck از مقدار `PORT` سرویس استفاده می‌کند و برنامه باید روی `0.0.0.0:$PORT` گوش دهد. citeturn0search0turn0search6
