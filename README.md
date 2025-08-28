# Worship & Yapps

_A quick start script is included for both Windows (PowerShell) and macOS/Linux (Bash). Use the one that matches your system._

A Calgary-based Bible study and community app. Browse discussion topics, discover local gatherings, build your network, and sign up for events — all in a simple mobile-first UI.

---

## ✨ Features
- Topics feed with swipeable discussion cards  
- Locations view for finding nearby groups and events  
- Community network directory  
- Email sign-up / onboarding flow  
- Toast notifications and smooth, responsive UI  

---

## 🧰 Tech Stack
- **Frontend:** React + TypeScript + Vite, Tailwind CSS, lucide-react icons  
- **State/UX:** react-hot-toast, date-fns  
- **Backend:** Supabase (auth + data)  
- **Build/Dev:** ESLint, PostCSS, Terser  

---

## 🚀 Quick Start (One-Command)

If you want everything handled for you, use the helper script. It will:
- check Node is installed,
- install dependencies,
- create a `.env` file if missing with placeholder values,
- then either start **dev mode** or do a **prod build + preview** (your choice).

### macOS / Linux
```bash
# from the project root after cloning
chmod +x scripts/one_command.sh
./scripts/one_command.sh dev     # starts vite dev server
# or
./scripts/one_command.sh build   # builds then starts preview server
```

### Windows (PowerShell)
```powershell
# from the project root after cloning
powershell -ExecutionPolicy Bypass -File scripts/one_command.ps1 dev
# or
powershell -ExecutionPolicy Bypass -File scripts/one_command.ps1 build
```

> The preview server serves the production build locally. Stop any running server with CTRL+C.

---

## 🔧 Manual Setup (if you prefer)

### 1) Prerequisites
- Node.js 18+ and npm (or pnpm/yarn)

### 2) Clone and install
```bash
git clone https://github.com/temiloluwua/worship-and-yapps.git
cd worship-and-yapps
npm install
```

### 3) Environment variables
Create a `.env` file in the repo root:
```bash
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 4) Run it locally
```bash
npm run dev
```
The app will start on http://localhost:5173.

### 5) Production build
```bash
npm run build
npm run preview   # serves the built app locally
```

---

## 📁 Project Structure
```
worship-and-yapps/
├─ index.html
├─ package.json
├─ postcss.config.js
├─ tailwind.config.js
├─ tsconfig.json
├─ vite.config.ts
├─ scripts/
│  ├─ one_command.sh
│  └─ one_command.ps1
└─ src/
   ├─ App.tsx
   ├─ main.tsx
   ├─ index.css
   ├─ components/
   │  ├─ Header.tsx
   │  ├─ BottomNavigation.tsx
   │  └─ ... (topics, locations, network, signup)
   └─ hooks/
      └─ useAuth.ts
```

---

## 🛠️ Scripts
- `npm run dev` – start Vite dev server  
- `npm run build` – type-check + bundle for production  
- `npm run preview` – preview production build  
- `npm run lint` – ESLint check  

---

## 🌐 Meta tags & Sharing
The app includes Open Graph/Twitter tags for rich previews. Update these if your domain or images change (see `index.html`).  

---

## 🗺️ Roadmap
- [ ] Real location map with pins  
- [ ] Event RSVP and reminders  
- [ ] Admin tools for posting topics/events  
- [ ] Profile pages and DMs  
- [ ] Accessibility pass (keyboard nav + ARIA)

---

## 🤝 Contributing
Issues and PRs are welcome! Please open an issue to discuss any major changes first.

---

## 📝 License
Add a LICENSE file (MIT is common for apps like this). If you intend to keep it closed-source, note that here.

---

## 🙌 Acknowledgments
Thanks to the Calgary faith community and everyone testing early builds.
