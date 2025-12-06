---
marp: true
theme: gaia
paginate: true
_paginate: true
size: 16:9
header: 'AcmeFlow v2.4 – Product Documentation'
footer: '23f1001996@ds.study.iitm.ac.in'
style: |
  section { font-family: "Inter", sans-serif; }
  section.lead { justify-content: center; text-align: center; }
  h1 { color: #0ea5e9; }
  h2 { color: #38bdf8; }
  code { background: #1e293b; padding: 0.2em 0.4em; border-radius: 6px; }
  pre { background: #0f172a; }
---

<!-- 
  Marp directives used in this slide:
  - _backgroundImage
  - _class
  - _paginate (inherited from front-matter)
  - _color (custom text color)
-->
<!-- _backgroundImage: url('https://images.unsplash.com/photo-1451187580459-43490279c0fa?q=80&w=2072&auto=format&fit=crop') -->
<!-- _class: lead -->
<!-- _color: #ffffff -->

# AcmeFlow v2.4
### Product Documentation Presentation

Built with **Marp** – Markdown → Slides → Git-friendly

---

# Why Marp for Technical Documentation?

- 100% plain Markdown in Git
- Instant HTML, PDF, PPTX export
- Full version control & diff-friendly
- LaTeX math, Mermaid diagrams, code highlighting
- Custom themes & CSS in the same repo

---

# Core Architecture

```mermaid
graph LR
    A[Web / Mobile Apps] --> B[API Gateway]
    B --> C[Auth Service]
    B --> D[Workflow Engine]
    D --> E[Task Queue<br/>(Kafka)]
    D --> F[(PostgreSQL)]
    D --> G[Redis Cache]
