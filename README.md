You are a senior full-stack engineer. Improve and complete my existing React + TypeScript web app (Apple Notes–style UI) with clean architecture, modular code, and production-level behavior.

Follow this exact implementation order:

---

1. ROUTING & SIDEBAR NAVIGATION

- Fix and implement routing using React Router.
- Sidebar items must route correctly:
  - All Meetings
  - Action Items
  - Decisions
  - Discussion
  - Problems
- Routing should be dynamic and filtered based on note category.
- Each route displays only relevant categorized notes.

---

2. NOTE SYSTEM (CORE LOGIC)

- Implement full CRUD:
  - Create new note
  - View note
  - Delete note
- Clicking a note should:
  - Expand into a detailed full view
  - Show complete content (not preview)
- Notes should be structured with:
  - Title
  - Content
  - Category
  - Timestamp

---

3. AI CATEGORIZATION ENGINE

- Build a smart categorization function (no external API required).
- It should:
  - Detect keywords (e.g., "decide", "issue", "task")
  - Understand intent/meaning (basic NLP logic)
- Automatically classify notes into:
  - Action Item
  - Decision
  - Discussion
  - Problem
- Make it modular so it can be replaced later with real AI.

---

4. SUMMARY PANEL

- Display dynamic counts:
  - Total notes
  - Action Items count
  - Decisions count
  - Problems count
- Update in real-time when notes change.

---

5. SHORTCUTS (HIDDEN BUT FUNCTIONAL)

- Remove shortcuts UI from display.
- Keep functionality:
  - "New Note" trigger should still work programmatically.

---

6. SHARE FUNCTIONALITY

- Remove global "Share" button at top.
- Add share button inside each note.
- Clicking share should:
  - Share only that specific note
  - Use Web Share API (fallback to copy link/text)

---

7. AUTHENTICATION (BASIC)

- Create login page:
  - App name: "Debrief"
  - Fields:
    - Email
    - Password
- Simple local authentication (no backend required):
  - Store session in localStorage
- Protect main app routes (redirect if not logged in)

---

8. UI / UX IMPROVEMENTS

- Maintain Apple Notes–style minimal UI.
- Ensure:
  - Clean spacing
  - Large readable typography
  - Smooth note expansion animation
- Keep components modular and reusable.

---

9. CODE QUALITY

- Use:
  - Functional components
  - Hooks
  - Clean folder structure
- Separate:
  - UI
  - Logic
  - State
- Avoid unnecessary re-renders.

---

Output Requirements:

- Provide updated code (not explanations unless necessary)
- Keep code clean, readable, and minimal
- Prioritize working functionality over overengineering
