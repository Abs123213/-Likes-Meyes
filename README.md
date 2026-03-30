# Free Fire Like API  

A simple API for **Send Like to Garena Free Fire Accounts**  
Built with **Flask** for lightweight, fast, and reliable performance.

---

## 🌟 Features
- Decode **Free Fire JWT tokens** instantly to find player region.
- Fetch **player details** and automatically manage `lock_region`.
- Automatically send requested Likes using dynamically updated tokens.
- Fully **asynchronous** internal requests for maximum speed.
- Easy deployment on **Vercel** (serverless, free hosting)  

---

## 🚀 Deploy to Vercel  

Click below to deploy directly to **Vercel**:  

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/itz-paglu/Free-Fire-Like-API)  

### After Deploying
1. Your project will automatically rely on `uidpass.json` and `tokens.json`.
2. Ensure you have run the update script or set up the GitHub Workflow to periodically refresh `tokens.json`.
3. Your Vercel domain (e.g., `https://free-fire-like-api.vercel.app`) is now serving your API endpoints!

✅ Save changes and redeploy if necessary. Your API is now ready!

---

## 🔗 Endpoint Usage

After deploying to Vercel (or running locally), you can hit your API via simple HTTP requests:

**GET** `/like`

**Query Parameters:**
- `uid` (Required): The Free Fire Player ID to send likes to.
- `server_name` (Optional): Force a specific region (e.g., `IND`, `BD`, `BR`). If omitted, it will automatically parse the `lock_region` from your active token!

### Example Request:
```bash
https://your-domain.com/like?uid=123456789
```

### Example Response:
```json
{
  "credit": "https://t.me/paglu_dev",
  "LikesGivenByAPI": 100,
  "LikesafterCommand": 200,
  "LikesbeforeCommand": 100,
  "PlayerNickname": "PlayerName",
  "Region": "BD",
  "UID": 123456789,
  "status": 1
}
```

---

## 📊 Repository Stats  

<p align="center">
  <img src="https://img.shields.io/github/stars/itz-paglu/Free-Fire-Like-API?style=for-the-badge&logo=github&color=yellow" />
  <img src="https://img.shields.io/github/forks/itz-paglu/Free-Fire-Like-API?style=for-the-badge&logo=github&color=blue" />
  <img src="https://img.shields.io/github/contributors/itz-paglu/Free-Fire-Like-API?style=for-the-badge&logo=github&color=green" />
  <img src="https://komarev.com/ghpvc/?username=itz-paglu&repo=Free-Fire-Like-API&style=for-the-badge&color=red" />
</p>  

---

## 💛 Credits  

<p align="center">
  <a href="https://t.me/itzpaglu">
    <img src="https://img.shields.io/badge/Owner-🔥%20@itzpaglu-pink?style=for-the-badge&logo=telegram" />
  </a>
  <a href="https://t.me/paglu_dev">
    <img src="https://img.shields.io/badge/Channel-TARIKUL.dev-blue?style=for-the-badge&logo=telegram" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/itz-paglu/Free-Fire-Like-API/stargazers" target="_blank">
    <img src="https://img.shields.io/badge/⭐%20Star%20This%20Repo-yellow?style=for-the-badge&logo=github" />
  </a>
</p>
