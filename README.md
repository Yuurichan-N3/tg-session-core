<div align="center">

<img width="100%" alt="header" src="https://capsule-render.vercel.app/api?type=waving&height=210&text=TG%20Session%20Core&fontAlign=50&fontAlignY=35&fontSize=54&desc=Multi-Session%20Telegram%20Tools%20(%20EXE%20Release%20)&descAlign=50&descAlignY=58"/>

<img alt="typing" src="https://readme-typing-svg.demolab.com?font=Inter&size=18&duration=3200&pause=650&center=true&vCenter=true&width=900&lines=Multi-session+Telegram+automation+tools;Extract+WebApp+initData+%7C+Join%2FLeave+%7C+Reaction+%7C+2FA;NEW%3A+Auto+Solve+Math+Quiz+%7C+Auto+Click+Inline+%7C+Auto+Chat"/>

<p>
  <img alt="telegram" src="https://img.shields.io/badge/Telegram-Session%20Tools-26A5E4?logo=telegram&logoColor=white"/>
  <img alt="windows" src="https://img.shields.io/badge/Windows-EXE%20Release-0078D4?logo=windows&logoColor=white"/>
  <img alt="multi-account" src="https://img.shields.io/badge/Multi-Account-111111"/>
  <img alt="license" src="https://img.shields.io/badge/License-Key%20Required-111111"/>
</p>

<p>
  <b>tg-session-core</b> adalah toolkit Telegram berbasis <i>session</i> untuk kebutuhan utilitas (multi akun, extract initData, manage chat, dan mode auto).
  Project ini didistribusikan sebagai <b>EXE</b> bernama <b>Yuurigram.exe</b>.
</p>

</div>

---

## 🚀 Download (EXE Release)

- **Latest EXE (Google Drive):** <a href="https://drive.google.com/file/d/15CInvp5MHD6aW5c9uEv3IwmWM6MZK25_/view?usp=sharing"><b>Download Yuurigram.exe</b></a>
- **Ambil LICENSE Key:** <a href="https://t.me/SentinelicenseBot?start=6004380466"><b>SentinelicenseBot</b></a>

---

## ⚡ Quick Start (EXE)
1) Download EXE dari bagian **Download (EXE Release)**  
2) Jalankan EXE → masukkan **LICENSE Key**  
3) Isi `APP_ID` & `APP_HASH` (bisa via prompt, atau taruh di file `.env`)  
4) Semua session akan tersimpan di folder **`Session/`** (auto dibuat)  
5) Jalankan fitur yang kamu butuhkan dari menu

> Tips: kalau kamu pakai banyak akun, pastikan file `*.session` ada di folder `Session/`.

---

## 🖼️ Preview

<div align="center">
  <img src="image/image.png" alt="Yuurigram Preview" width="900" />
</div>

---

## ✨ Fitur Utama

### ✅ Session & Account
- **Create New Session** (login, simpan ke folder `Session/`)
- **Check Account / Session Status** + optional extract:
  - `number.txt` (phone)
  - `userid.txt` (user id)
- **Get Latest Telegram Login Message** (OTP / pesan terbaru)

### ✅ WebApp / InitData
- **Auto Extract InitData (tgWebAppData)**:
  - output `query.txt` (raw)
  - output `user.txt` (user param diprioritaskan)

### ✅ Group/Channel Tools
- **Auto Join Groups/Channels** (support link public + invite `t.me/+...`)
  - optional: **mute** setelah join
  - optional: **archive** setelah join
- **Auto Leave Groups/Channels** (support `@username`, link, `-100...`, numeric)

### ✅ Chat Management
- **Mute all chats** / **Unmute all chats**
- **Archive selected groups/channels**
- **Block & Delete selected users/chats**

### ✅ Profile & Security
- **Auto Edit Name** (replace/append first/last, delete last name)
- **Auto Set 2FA** (hanya jika akun belum punya 2FA)

### ✅ Engagement
- **Auto Reaction** (pilih 1 emoji atau random dari list)

---

## 🆕 Fitur Baru (Auto Mode)

### 🧮 Auto Solve Math Question (Inline Math Quiz Engine)
Mode tersedia:
1. **Click inline dulu**, lalu jawab math dari pesan itu
2. **Jawab math dulu**, lalu klik inline konfirmasi (smart wait 5 detik di akun pertama)
3. **Langsung jawab math** dari last message (tanpa inline handling)


### 🖱️ Auto Click Inline
- Scan last message dari bot target untuk menemukan inline buttons
- Pilih tombol ke-berapa (sekali), lalu tool akan klik tombol itu di semua session

### 💬 Auto Chat (Random / Custom)
Auto chat ke bot target dengan berbagai tipe pesan:
- Random link:
  - X profile / tweet
  - Facebook profile / post
  - TikTok profile / post
  - Instagram profile / story / post / reels
  - YouTube profile / video / shorts
- Username mode:
  - Random username style (DC/X/TELE/IG/TT/FB) + opsi pakai `@` atau tidak
  - Telegram username real (kalau ada) atau random
- **Custom text** (kirim persis input kamu)
- **Crypto address**:
  - EVM / Solana / TRX  
  - ⚠️ Address dikirim ke chat, **private key disimpan lokal** ke `Privatekey/privatekey.json`

---

## 🧭 Menu (Versi Script Terbaru)
```text
01. Create New Session
02. Auto Extract InitData
03. Auto Join Groups/Channels
04. Auto Leave Groups/Channels
05. Auto Referral Bot (/start + ref)
06. Auto Edit Name (First/Last - replace/append/delete)
07. Auto Reaction (single/random)
08. Check Account or Session Status & Extract Data
09. Setting Chat (Mute/Unmute All, Archive Selected, Block/Delete)
10. Auto Set 2FA (only for accounts without 2FA)
11. Get Latest Telegram Login Message
12. Auto Solve Inline Math Questions
13. Auto Click Inline Button
14. Auto Chat (links, usernames, YouTube, crypto)
15. Exit
```

---

## 📁 Struktur Folder & Output
```text
tg-session-core/
├─ Yuurigram.exe
├─ .env                 # optional (APP_ID, APP_HASH)
├─ Session/             # tempat file *.session (multi account)
├─ Privatekey/
│  └─ privatekey.json   # output auto chat crypto (private key disimpan di sini)
├─ query.txt            # output initData raw
├─ user.txt             # output initData (user param di depan)
├─ number.txt           # optional output phone
└─ userid.txt           # optional output user id
```

---


## 🧯 Notes (Anti-Flood)
- Kalau kena **FloodWait**, itu normal (Telegram limit).  
- Pakai akun banyak + spam action = resiko limit lebih tinggi.

---

## ⚠️ Disclaimer
Project ini dibuat untuk keperluan pribadi / automation workflow.  
Gunakan dengan bijak dan tetap patuhi aturan Telegram serta aturan grup/channel yang kamu join.

---

<div align="center">
<img width="100%" alt="footer" src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer"/>
</div>
