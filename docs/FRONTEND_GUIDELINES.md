# Frontend Guidelines (Quick Cheat-Sheet) 🎨

> Keep it simple: **Clean Tailwind, shared Lego blocks, and real backend data.**

---

## The 4 Rules
1. **Tailwind Only:** No new `.css` files. Use utility classes (`p-4`, `bg-slate-900`, `rounded-xl`).
2. **Reuse Atoms First:** Look inside `src/components/common/` before styling buttons or cards from scratch.
3. **No Mock Data:** The backend has real data ready. Fetch it via `src/services/`.
4. **Clean Code:** Always test `npm run build` before pushing.

---

## Folder Organization
```text
src/
├── components/
│   ├── common/      # Reusable blocks (Button, Badge, Modal, Input)
│   ├── layout/      # Navbar, Sidebar, DashboardLayout
│   ├── student/     # Student-specific components
│   └── tpo/         # TPO-specific components
├── pages/           # Main route screens
├── services/        # Axios API calls
└── context/         # AuthContext
```

---

## Standard Component Skeleton
```jsx
// src/components/common/Card.jsx
export default function Card({ title, children }) {
  return (
    <div className="bg-white rounded-xl border border-slate-200 shadow-sm p-6">
      {title && <h3 className="text-lg font-bold text-slate-900 mb-4">{title}</h3>}
      {children}
    </div>
  );
}
```
