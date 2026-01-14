# Boutique Legal Counsel Website Roadmap (MVP → v1 → v2)

## Assumptions & Principles
- Mobile-first, accessible (WCAG 2.1 AA) UI with Matrix-inspired geometry and restrained motion.
- TR/EN bilingual content at launch (MVP), with scalable i18n for future locales.
- Backend via Bolt-compatible stack (tables, storage, RLS, admin auth) with strict least-privilege policies.
- Performance targets: LCP < 2.5s on mobile, CLS < 0.1, minimal blocking scripts.

---

## MVP (Foundational Presence + Core Intake)
**Target**: 4–6 weeks  
**Goal**: Public marketing site, bilingual content, basic intake & contact pipeline.

### Scope
1. **Design System**
   - Tailwind config with Matrix palette (greens/blacks/grays), typography (Inter), component tokens.
   - Base geometric UI library (cards, dividers, angled sections).
2. **Core Pages**
   - Home, About, Expertise, Team, Contact.
   - Basic Legal Insights listing (static or minimal CMS-backed).
3. **Internationalization**
   - TR/EN toggle, locale persistence, translations for all static pages.
4. **Forms & Intake**
   - Contact form + multi-step case application form (name, email, phone, case summary, urgency).
   - Validation + confirmation screen with tracking number.
5. **Backend (Minimal)**
   - Tables: users, case_applications, contact_submissions.
   - Storage bucket for uploads (document intake).
   - RLS policies for secure access.
6. **Animations**
   - Subtle reveal-on-scroll, geometric hover states, basic hero background motion.

### Deliverables
- Live MVP site with bilingual content.
- Secure intake pipeline and storage for documents.
- Lightweight analytics or basic event tracking.

---

## v1 (Content Authority + Rich Experience)
**Target**: +6–8 weeks  
**Goal**: Thought leadership hub, richer interactions, improved UX depth.

### Scope
1. **Legal Insights & Blog**
   - 8–10 doctoral-level strategic articles (AI regulation, data sovereignty, crypto, etc.).
   - Blog listing with filtering, tags, search, category badges.
   - Article detail templates with rich typography and references.
2. **Expertise Enhancements**
   - Filter/search on practice areas, expandable details, success metrics snippets.
   - Custom geometric Lucide-based iconography.
3. **Advanced Interaction**
   - Scroll-based parallax and geometric transitions between sections.
   - Improved hover/micro-interactions, loading states.
4. **Backend Expansion**
   - Tables: blog_posts, legal_insights.
   - Admin CRUD for posts, image uploads, preview.

### Deliverables
- Full content hub with bilingual posts.
- Usable admin interface for content management.
- Measurable UX improvements (animations, navigation, filters).

---

## v2 (Operational Scale + Compliance & Insights)
**Target**: +6–10 weeks  
**Goal**: Operational dashboard, analytics, deeper compliance features.

### Scope
1. **Admin Dashboard**
   - Protected routes, application review pipeline, document management.
   - Notifications for new submissions.
2. **Compliance & Security**
   - Enhanced audit logs, retention policies, access reviews.
   - SOC 2-aligned controls and documentation.
3. **UX/Performance Refinement**
   - Deep performance optimization, lazy loading, advanced caching.
   - Accessibility audit and remediation.
4. **Growth Features**
   - Related content recommendations.
   - Localization expansions beyond TR/EN if needed.

### Deliverables
- Operationally scalable admin panel.
- Compliance posture improvements (policies + observability).
- Performance and accessibility hardened release.

---

## Estimated Effort (Rough Order)
| Phase | Design | Frontend | Backend | Content | QA/Perf | Total |
|------|--------|----------|---------|---------|---------|-------|
| MVP  | 1–2 w  | 2–3 w    | 1–2 w   | 1–2 w   | 1 w     | 4–6 w |
| v1   | 1–2 w  | 3–4 w    | 2–3 w   | 2–3 w   | 1–2 w   | 6–8 w |
| v2   | 1–2 w  | 3–4 w    | 3–4 w   | 1–2 w   | 2 w     | 6–10 w |

---

## Dependencies / Inputs Needed From You
- Final brand assets (logo, typography preferences, palette direction).
- Approved TR/EN copy for core pages.
- Decision on backend provider (Bolt/Supabase/other).
- Legal content source or review process for doctoral-level articles.
- Compliance expectations (KVKK/GDPR/SOC 2 level).

