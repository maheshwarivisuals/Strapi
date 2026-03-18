# 🚀 Strapi Auto SSL Deployment (Docker)

Production-ready Strapi CMS with:
- Auto SSL (Let's Encrypt)
- Dockerized Nginx Proxy Manager
- PostgreSQL

---

## ⚡ Quick Deploy

### 1. Clone repo
git clone https://github.com/maheshwarivisuals/strapi
cd strapi-auto-ssl

### 2. Setup env
cp 1.env .env
nano .env

### 3. Run
docker compose up -d

---

## 🌐 Access

Nginx Proxy Manager:
http://YOUR_SERVER_IP:81

Default login:
admin@example.com
changeme

---

## 🔗 Connect Domain

1. Login to Nginx Proxy Manager
2. Go to "Proxy Hosts"
3. Add new:
   - Domain: blog.maheshwarivisuals.com
   - Forward Host: strapi_app
   - Port: 1337

4. Enable:
   ✅ Websockets
   ✅ Block Common Exploits

5. SSL Tab:
   ✅ Request new SSL
   ✅ Force HTTPS

DONE 🎉

---

## ⚠️ Important

- Change default login immediately
- Use strong DB password
- Backup volumes regularly

---

## 🧠 Notes

Strapi runs internally, not exposed publicly.
Only Nginx handles traffic + SSL.

---

Built for fast production deployment 🚀
