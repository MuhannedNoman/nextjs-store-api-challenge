# Front-End Coding Challenge (Next.js + Platzi Fake Store API)

Welcome! This challenge helps us evaluate how you build a small, production-like front-end feature set using **Next.js**.

You will build a simple product browsing experience using:
- **Next.js (App Router preferred)**
- Public API: https://fakeapi.platzi.com/en

---

## ✅ What You’ll Build

A small web app with:
1. **Products List** (with filtering, search, and pagination)
2. **Product Details** page
3. Solid UX states: loading, empty, error

---

## 🎯 Objectives (What We’re Evaluating)

We’ll look for:
- Clean, maintainable component structure
- Good UX and attention to detail
- Data fetching patterns and caching
- Performance considerations (rendering, loading states, image optimization)
- Correct handling of edge cases
- TypeScript (Optionally) usage and code quality
- Practical styling and responsiveness

---

## 📌 Requirements

### 1) Pages / Routes

#### A) Products List Page
Route: `/` (or `/products`)

Features:
- Display products in a grid (responsive).
- Each product card should show:
  - Image
  - Title
  - Price
  - Category name
- **Category Filter**
  - Fetch and display categories.
  - Allow filtering products by category.
- **Search**
  - Search by product title (case-insensitive).
  - Should not feel laggy (debounce is recommended).
- **Pagination**
  - Implement pagination using `offset` + `limit` in the UI logic.
  - Provide “Next” / “Previous” or page numbers.
- Handle:
  - Loading state
  - Error state
  - Empty state (no results)

#### B) Product Details Page
Route: `/products/[id]`

Features:
- Display:
  - Title
  - Images (one main image is OK)
  - Price
  - Description
  - Category info
- Handle loading + error state
- Include a “Back to products” action

---

## 🔌 API Endpoints (External)

Use the Platzi Fake Store API.

Suggested endpoints you may need (based on API docs):
- Categories list
- Products list
- Product details

> You can call the API directly from Next.js (server components or route handlers are both acceptable).

---

## 🧠 Technical Expectations

### Next.js
- Prefer **Next.js App Router** (`app/`).
- Use TypeScript (Optionally).
- Use Next Image (`next/image`) where applicable.
- Choose one approach for data fetching and be consistent:
  - Server Components + `fetch`
  - Client Components + React Query
  - Or a hybrid (document your choice)

### Styling
- Tailwind is preferred and any UI component
- Must be responsive and clean.

### Code Quality
- Reasonable folder structure
- Reusable components where it makes sense
- Avoid over-engineering

---

## ⭐ Bonus (Optional but Valuable)

Pick any 2–4:
- Sort products (price / title)
- Debounced search
- Skeleton loaders
- URL-synced filters (query params like `?category=2&search=chair&page=2`)
- Accessibility improvements (keyboard navigation, aria labels)
- Auth since the API support a simple authentication.
- Deployment on any platform

---

## 📦 Submission

Please provide:
A public GitHub repository link (or zipped project)
A short note in the README including:
How to run it
Key technical decisions (data fetching approach, state management, etc.)
Tradeoffs and what you’d improve with more time

---

## ⏱️ Time Expectation

Focus on correctness and clarity over perfection.
Good luck — we’re excited to see your approach!
