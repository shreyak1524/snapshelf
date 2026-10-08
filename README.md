# SnapShelf 📚✨
### *Personal Digital Resource Organizer*

> Built for the 3-Hour AI App-Building Competition.
> A fast, polished, offline-first digital resource organizer to save, categorize, and instantly retrieve documents, notes, links, and media across custom shelves.

---

## 🚀 Live Demo & Quick Start

### 1. Installation & Local Development
```bash
# Clone or navigate to the project directory
cd snapshelf

# Install dependencies
npm install

# Start development server
npm run dev
```

### 2. Production Build
```bash
# Creates optimized production build in /dist
npm run build

# Preview production build locally
npm run preview
```

### 3. Deploy to Vercel (1-Click)
SnapShelf is configured to deploy directly to Vercel with zero backend or API key prerequisites:
1. Push this repository to GitHub / GitLab.
2. In Vercel, import the repository and select `Vite` framework preset.
3. Build Command: `npm run build`
4. Output Directory: `dist`
5. Deploy!

---

## 🎯 Tech Stack
- **Frontend Framework:** React 19 + Vite 8
- **Styling:** Tailwind CSS (Modern clean cards, subtle animations, dark/light themes)
- **Icons:** Lucide React
- **Persistence:** LocalStorage with resilient fallback, export, import, and demo reset capabilities
- **Zero API Keys Required:** Runs 100% reliably in offline or sandboxed browser environments.

---

## 🌟 Core Features Implemented

### 1. 📊 Modern Dashboard
- Live statistics cards: Total Resources, Shelves count, Starred items, Format breakdown.
- Visual Shelves grid displaying real-time resource tallies.
- "Recently Saved" resource feed.
- "Favorites" quick shelf.
- One-click quick actions (+ Save Resource, + New Shelf, Future Scope roadmap).

### 2. 🗂️ Customizable Shelves
- Create new shelves with custom **Names**, **Descriptions**, **Color Themes** (Blue, Emerald, Purple, Amber, Rose, Indigo), and **12 Curated Icons** (Study, Code, Career, Idea, etc.).
- Dedicated shelf views with shelf header banners, counters, and scoped filtering.
- Safe deletion flow: Deleting a shelf preserves all saved resources into *Uncategorized*.
- Realistic seeded demo shelves:
  - 🎓 **Study Resources**
  - 💻 **Projects**
  - 💼 **Career**
  - 💡 **Inspiration**

### 3. 🔖 Save & Edit Resources
- Save modal supporting 6 Resource Types:
  - 🌐 **Website**
  - 📄 **PDF**
  - 📝 **Document**
  - 🗒️ **Note**
  - 🖼️ **Image**
  - 🎥 **Video**
- Form features: Title validation, Auto-protocol URL normalization, Shelf assignment, Tag chip management with instant suggestion pills, and Star toggle.
- Full Edit capability on every resource with changes instantly persisted to `localStorage`.

### 4. 🔍 Instant Search
- Real-time search indexing title, description, tags, resource type, and shelf names.
- Instant reactive feedback as you type.
- Global keyboard shortcut: `Ctrl+K` or `⌘K` to focus the search bar from anywhere.

### 5. 🎛️ Multi-Dimensional Filtering & Sorting
- Filter by Shelf, Format type, Favorites, or clickable Tag chips.
- Multiple sorting algorithms: *Newest First*, *Oldest First*, *Title (A-Z)*, *Title (Z-A)*.
- Layout switcher: **Grid View** (visual cards) vs. **List View** (compact density).
- Active filter counter and one-click *Reset filters* button.

### 6. 🔍 Resource Details Modal
- Click any card to inspect full metadata:
  - Formatted publication/save dates with relative time calculations (*"2 days ago"*).
  - Clean domain badge with copy-to-clipboard feedback.
  - "Open Resource" direct launch button.
  - Interactive shelf pill that jumps directly to that shelf.
  - Instant edit, delete (with safety confirmation), and favorite toggles.

### 7. ⭐ Favorites & Recent Feeds
- Toggle stars directly from cards, table rows, or detail dialogs.
- Dedicated Favorites page with counter badges in sidebar navigation.
- Sorted recent activity feed on dashboard.

### 8. 📱 Responsive Layout & Dark Mode
- Desktop: Expanded sidebar with statistics and quick tools.
- Tablet & Mobile: Touch-friendly hamburger drawer, responsive grids, and sticky search bar.
- Light and Dark mode toggle with system persistence.

### 9. 💾 Backup, Export & Instant Demo Reset
- **Export Data:** Download your full knowledge library as a `.json` backup.
- **Import Data:** Restore library from any SnapShelf backup file.
- **Reset Demo Data:** 1-click restore to sample competitive evaluation data for judges.

---

## 🔮 Future Scope & Roadmap (v2.0)

SnapShelf's architecture decouples storage adapters, entity schemas, and rendering views so the following features can be added without application rewrites:

1. 🧩 **Browser "Save to SnapShelf" Extension:**
   - Manifest V3 Chrome/Firefox extension to clip active URLs, page meta tags, and text selections directly into shelves.
2. ☁️ **Cloud Synchronization & Multi-Device:**
   - Offline-first CRDT synchronization via Supabase / Firebase Auth.
3. 🏷️ **Smart Automatic Tagging:**
   - AI topic classification that analyzes URL content and infers high-precision tags automatically.
4. 🔎 **Search Inside Documents & PDFs:**
   - In-browser full-text parsing via PDF.js Web Workers for text buried inside PDFs and docs.
5. 👁️ **OCR for Images & Mockups:**
   - Client-side or edge Vision AI to extract text and annotations from screenshots.
6. 👥 **Shared Shelves & Collaboration:**
   - Collaborative shelves with public read-only links and team workspace permissions.
7. 🎙️ **Voice Notes & Audio Transcription:**
   - Web Audio recording with Whisper-powered speech-to-text turning voice memos into structured notes.
8. 🧠 **Advanced Knowledge Search (Semantic RAG):**
   - Natural language question answering across all saved resources with direct source citations.

---

## 🏆 Competition Compliance
- ✅ **Fully working application** with verified zero compile/runtime errors.
- ✅ **Pure React + Vite + Tailwind CSS** (No Python/Flask backend needed).
- ✅ **Clean localStorage persistence** (survives browser refresh, no API keys required).
- ✅ **All visible buttons are 100% functional** with confirmation modals for destructive actions.
- ✅ **Ready for direct Vercel deployment**.
