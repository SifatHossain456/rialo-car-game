# Rialo — Car Avoid (Logo + Shield)

**একটি একদম সহজ, single-file HTML গেম** — যেখানে আপনি গাড়ি (লোগো) বামে-ডানে সরিয়ে উপরে থেকে আসা বাধা এড়িয়ে চলবেন। লোগো-কয়েন ধরলে **Shield power-up** অন হবে (৬ সেকেন্ড invincible), HUD-এ টাইমডাউন দেখা যাবে।

> 🔗 **Live (GitHub Pages)**: Settings → Pages → Branch: `main` → Save (ডেপ্লয় হলে লিঙ্ক হবে `https://<username>.github.io/<repo>/`)

---

## 🎮 Features
- **Single file**: পুরো গেমটা `index.html`-এর মধ্যে (HTML+CSS+JS)।
- **Logo integration**: গেম, মেনু, HUD এবং power-up-এ কাস্টম লোগো ব্যবহার।
- **Shield power-up**: লোগো-কয়েন ধরলে ৬ সেকেন্ডের শিল্ড (ভিজ্যুয়াল রিং + HUD কাউন্টডাউন)।
- **Difficulty ramp**: সময়ের সাথে গতি ও স্পন ফ্রিকোয়েন্সি বেড়ে যায়।
- **Best score**: ব্রাউজারের `localStorage`-এ সেভ থাকে।
- **Mobile friendly**: টাচ বোতামসহ।

---

## ⌨️ Controls
- **Start / Pause**: বোতাম থেকে বা **Enter**
- **Move**: **← →** বা **A / D**
- **Restart**: **R**

---

## 🛠️ Run Locally
1. এই রিপো থেকে `index.html` ডাউনলোড/ক্লোন করুন।
2. ফাইলটায় **ডাবল-ক্লিক** করলেই ব্রাউজারে গেম চলবে।
   - বিকল্প: টার্মিনাল থেকে ছোট HTTP সার্ভার চালাতে পারেন:
     ```bash
     # Python 3
     python -m http.server 8000
     # তারপর ব্রাউজারে খুলুন: http://localhost:8000/index.html
     ```

---

## 🚀 Deploy (GitHub Pages)
1. এই রিপোজিটরিতে `index.html` commit/push করুন।
2. **Settings → Pages → Branch:** `main` নির্বাচন করুন, **Save**।
3. কিছুক্ষণের মধ্যে লাইভ লিঙ্ক হবে: `https://<username>.github.io/<repo>/`

---

## 🗂️ Project Structure
```
repo/
└─ index.html   # গেমের সম্পূর্ণ সোর্স (HTML+CSS+JS)
```
> নোট: এই ভার্সনে লোগো **embedded data URL** হিসেবে যুক্ত (index.html-এর ভেতরেই), আলাদা ফাইল লাগবে না।

---

## 🧩 Customization
- **লোগো বদলাতে** চাইলে `index.html`-এ `logo.src = "data:image/...base64,..."` অংশটি নতুন data-URL বা ফাইলপথে বদলে দিন।
- **লেনে সংখ্যা**: `lanes` ভ্যারিয়েবল (ডিফল্ট `3`)।
- **শিল্ড সময়**: `activateShield(6000)` → মিলিসেকেন্ডে সময়।
- **স্পিড/ডিফিকাল্টি**: `speed`, `diffMult` ও `spawnEvery` লজিক।
- **কালার থিম**: CSS `:root` ভ্যারিয়েবলগুলো (`--bg`, `--road`, `--lane`, `--accent`, `--good` ইত্যাদি)।

---

## 🤝 Contributions
PR স্বাগত! বাগ/আইডিয়ার জন্য Issue খুলুন।

---

## 📜 License
MIT (নিজ দায়িত্বে ব্যবহার করুন; এম্বেড করা লোগোর মালিকানা/ব্যবহারের দায় ব্যবহারকারীর)।

