<div align="center">

<img width="100%" alt="header" src="https://capsule-render.vercel.app/api?type=waving&height=210&text=Yuurigram%20(EXE)&fontAlign=50&fontAlignY=36&fontSize=56&desc=Telegram%20Session%20Tools%20%7C%20Multi%20Account%20Automation&descAlign=50&descAlignY=58"/>

<img alt="typing" src="https://readme-typing-svg.demolab.com?font=Inter&size=18&duration=3000&pause=650&center=true&vCenter=true&width=900&lines=Create+%26+Manage+Telegram+Sessions;InitData+Extractor+(tgWebAppData);Auto+Join%2FLeave%2FReferral%2FReaction%2F2FA%2FOTP;Auto+Math+Solve+%7C+Auto+Click+Inline+%7C+Auto+Chat+%7C+Auto+Giveaway+Join"/>

<p>
  <img alt="telegram" src="https://img.shields.io/badge/Telegram-Tools-26A5E4?logo=telegram&logoColor=white"/>
  <img alt="windows" src="https://img.shields.io/badge/Windows-EXE%20Release-0078D4?logo=windows&logoColor=white"/>
  <img alt="multi-account" src="https://img.shields.io/badge/Multi-Account-111111"/>
  <img alt="license" src="https://img.shields.io/badge/License-Required-111111"/>
</p>

<p>
  <b>tg-session-core</b> adalah toolkit Telegram berbasis <i>session</i> untuk kebutuhan utilitas (multi akun, extract initData, manage chat, dan mode auto).
  Project ini didistribusikan sebagai <b>EXE</b> bernama <b>Yuurigram.exe</b>.
</p>

</div>

---

## 🚀 Download (EXE Release)

- **Latest EXE (Google Drive):** <a href="https://drive.google.com/file/d/1os7fqwElXOucbh2-_DKBU5zUgSHce11t/view?usp=sharing"><b>Download Yuurigram.exe</b></a>  
- **Ambil LICENSE Key:** <a href="https://t.me/SentinelicenseBot?start=6004380466"><b>SentinelicenseBot</b></a>

---

## ⚡ Quick Start (EXE)

1) Download `Yuurigram.exe`  
2) Jalankan EXE → masukkan **LICENSE Key**  
3) Isi `APP_ID` & `APP_HASH` (bisa via prompt, atau taruh di file `.env`)  
4) Semua session akan tersimpan di folder **`Session/`** (auto dibuat)  
5) Pilih menu yang kamu butuhkan

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
- **Get Latest Telegram OTP Login Message** (cek pesan login terbaru)

### ✅ WebApp / InitData
- **Auto Extract InitData (tgWebAppData)**
  - output `query.txt` (raw)
  - output `user.txt` (user param di depan)

### ✅ Group / Channel Tools
- **Auto Join Groups/Channels** (support link / @username / invite)
  - opsi **mute** + **archive** setelah join
- **Auto Leave Groups/Channels** (bulk leave via list)

### ✅ Bot / Engagement
- **Auto Referral Bot** (`/start` + referral code opsional)
  - auto **mute** + **archive** bot setelah kirim
- **Auto Reaction** (pilih emoji tunggal / random dari list)

### ✅ Profile & Security
- **Auto Edit Name** (replace / append / delete last name)
- **Setting Chat**:
  - **Mute all** (yang belum mute)
  - **Unmute all**
  - **Archive selected**
  - **Block & delete selected**
- **Auto Set 2FA** (enable kalau belum set)

---

## 🆕 Fitur Baru (Auto Mode)

### 🧮 Auto Solve Math Question (Inline Math Quiz Engine)
Mode tersedia:
1. **Click inline dulu**, lalu jawab math dari pesan itu
2. **Jawab math dulu**, lalu klik inline konfirmasi (smart wait 5 detik di akun pertama)
3. **Langsung jawab math** dari last message (tanpa inline handling)

> Deteksi ekspresi sederhana: `a + b`, `a - b`, `a * b`, `a / b`, atau `a x b`.

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

### 🎁 Auto Giveaway Join (Auto Search + Auto Join)
- Tool akan **mencari giveaway yang aktif secara otomatis**, lalu **auto join** channel/grup yang dibutuhkan.
- Setelah join: auto **mute** + **archive**
- Sistem “mirror join”: akun pertama jadi “master”, akun lain tinggal ngikut join yang sama.

> Tidak perlu input daftar channel satu per satu — cukup jalankan mode ini, sisanya tool yang handle.

---

## 🧭 Menu

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
15. Auto Giveaway Join (auto search + auto join)
16. Exit
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
- Kalau kena **FloodWait**, biarin tool tunggu / skip sesuai kondisi.
- Kalau bot target terlalu sering spam protect, pakai jeda / jalankan bertahap.
- Pastikan akun kamu aman (jangan kebanyakan join dalam waktu singkat).

---

## ⚠️ Disclaimer
Tool ini dibuat untuk membantu automasi utilitas Telegram milik sendiri. Gunakan dengan bijak dan tanggung jawab masing-masing.
