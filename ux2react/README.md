
# 🚀 UX2React

UX2React is an AI-powered developer tool that **converts Figma designs into clean, responsive React JSX code** — helping frontend developers and startups save hours of UI work.

---

## 🧠 Features (MVP)
- 🔼 Upload Figma File Key
- 📥 Fetch Figma JSON using API
- 🧩 Parse design elements into JSX components
- 🎨 TailwindCSS layout mapping
- 💡 AI-powered component naming (coming soon)
- 📤 Export or copy JSX code
- 🔌 Optional Figma Plugin support

---

## 🗂️ Project Structure

```
ux2react/
├── apps/
│   ├── frontend/    # Next.js frontend UI
│   └── backend/     # Express backend with parsing + AI
├── libs/            # Shared constants, utils, types
├── plugins/         # Figma plugin (optional)
├── docs/            # Architecture and API notes
├── scripts/         # Dev or deployment scripts
```

---

## 🛠️ Tech Stack

- Frontend: React + Next.js + TailwindCSS
- Backend: Node.js + Express + TypeScript
- AI Integration: OpenAI (GPT-4 or GPT-3.5)
- Design API: Figma REST API
- Optional: Handlebars templating for JSX

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/yourname/ux2react.git
cd ux2react
```

### 2. Install dependencies
```bash
npm install --workspaces
```

### 3. Setup environment variables

Create `.env` in `apps/backend`:
```
PORT=5000
FIGMA_TOKEN=your_figma_token
OPENAI_API_KEY=your_openai_api_key
```

Create `.env.local` in `apps/frontend`:
```
NEXT_PUBLIC_API_URL=http://localhost:5000
```

### 4. Run backend
```bash
cd apps/backend
npx nodemon
```

### 5. Run frontend
```bash
cd apps/frontend
npm run dev
```

---

## 📬 API Routes (Backend)

| Route | Description |
|-------|-------------|
| `POST /generate` | Accepts Figma file key and returns JSX |
| `POST /ai-generate` | (Upcoming) Uses OpenAI to return smart components |

---

## 🧩 Plugin (Optional)

Located in `plugins/figma-plugin/`, this plugin helps users send selected layers directly to the backend for conversion.

---

## 📈 Future Features

- 🧠 AI-assisted layout interpretation (Flex/Grid)
- 📦 Export as reusable React component packages
- ✨ Theme customization
- 💵 Pro pricing & Stripe integration
- 📦 VS Code extension

---

## 📄 License

MIT License © 2025 
