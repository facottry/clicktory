# The Clicktory SEO Checklist 🚀

A battle-tested 10-point checklist for launching a SaaS that actually gets indexed.
Based on our experience building **[Clicktory](https://www.clicktory.in)**.

## 1. Technical Health
- [ ] **Sitemap.xml**: Ensure it's auto-generated and submitted to GSC.
- [ ] **Robots.txt**: Block admin routes, allow bots on public pages.
- [ ] **Canonical Tags**: Prevent duplicate content penalties (especially with `?params`).
- [ ] **JSON-LD Schema**: Semantic structure for Product, Breadcrumb, and Review.

## 2. On-Page Basics
- [ ] **Title Tags**: Format `Keyword | Brand` (e.g., "Best AI Tools | Clicktory").
- [ ] **Meta Descriptions**: Active voice, under 160 chars.
- [ ] **H1 Hierarchy**: Only ONE H1 per page. H2s for major sections.
- [ ] **Image Alt Text**: Descriptive text for accessibility and image search.

## 3. Performance Core Web Vitals
- [ ] **LCP (Largest Contentful Paint)**: Under 2.5s. Optimize robust hosting (R2/S3).
- [ ] **CLS (Cumulative Layout Shift)**: Under 0.1. Define image dimensions explicitly.
- [ ] **Mobile Responsiveness**: Google indexes Mobile-First. Test resizing.

## 4. Content Strategy
- [ ] **Programmatic Pages**: Generate pages from database entries (e.g., `/product/:slug`).
- [ ] **Internal Linking**: Link related products/categories (Cluster strategy).
- [ ] **Freshness**: Show "Last Updated" dates.

---
*Built with ❤️ by the team at [Clicktory](https://www.clicktory.in)*
