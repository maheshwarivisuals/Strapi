# Strapi Docker Deploy 🚀

Production-ready Strapi CMS using Docker + PostgreSQL + Nginx

## 📦 Setup

### 1. Clone repo
git clone https://github.com/YOUR_USERNAME/strapi-docker-deploy.git
cd strapi-docker-deploy

### 2. Setup environment
cp .env.example .env
nano .env

### 3. Start containers
docker compose up -d

### 4. Open Strapi
http://YOUR_SERVER_IP:1337/admin

---

## 🌐 Domain Setup

Edit nginx/default.conf:
Replace:
blog.maheshwarivisuals.com

Then restart:
docker compose restart

---

## 🔒 SSL (Recommended)

sudo apt install certbot python3-certbot-nginx
sudo certbot --nginx -d yourdomain.com

---

## 📊 Services

- Strapi CMS → Port 1337
- PostgreSQL → Internal
- Nginx → Reverse Proxy

---

## ⚡ Production Tips

- Change DB password
- Use strong secrets
- Enable firewall
- Backup DB regularly

---

Made for fast deployment 💻