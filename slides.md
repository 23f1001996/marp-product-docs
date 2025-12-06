---
marp: true
theme: custom-theme
paginate: true
pagestyle: true
header: '**Product Documentation – AcmeFlow v2.4**'
footer: 'Contact: 23f1001996@ds.study.iitm.ac.in'
class: invert
style: |
  section { font-family: "Fira Sans", sans-serif; }
  h1, h2 { color: #00a8cc; }
  code { background: #2d2d2d; padding: 2px 6px; border-radius: 4px; }
  pre { background: #1e1e1e; }
  .columns { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; }
  footer { color: #aaa; font-size: 0.6em; }
---

<!-- _backgroundImage: url("https://images.unsplash.com/photo-1518432031352-d6fc5c10da5a?q=80&w=2070&auto=format&fit=crop) -->
<!-- _class: invert lead -->

# AcmeFlow v2.4  
**Product Documentation**

Modern, scalable workflow automation platform

---

# Why Choose Markdown + Marp?

- Fully version-controlled (Git)
- Single source of truth
- Export to HTML, PDF, PPTX with one command
- Beautiful slides without PowerPoint lock-in
- Supports LaTeX, diagrams, code highlighting

---

# Core Architecture

```mermaid
graph TD
graph LR
    A[Client Apps] --> B[API Gateway]
    B --> C[Microservices]
    C --> D[(PostgreSQL)]
    C --> E[Redis Cache]
    C --> F[Kafka Queue]
