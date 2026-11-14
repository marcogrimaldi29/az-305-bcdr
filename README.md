# 🛡️ AZ-305: Migration, HA & BCDR — Deep Dive

### Study Notes Repository — 2026 Edition

[![GitHub Pages Live](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?logo=github)](https://marcogrimaldi29.com/az-305-bcdr/)
[![marcogrimaldi29.com](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)
[![AZ-305 Main Notes](https://img.shields.io/badge/AZ--305-Main%20Notes-blue?logo=microsoftazure)](https://marcogrimaldi29.com/az-305-study-notes/)

> - 🎯 **Goal:** Master High Availability, Backup, Disaster Recovery, and Migration for the **AZ-305** exam
> - 📅 **Notes Version:** 2026
> - 🌐 **Published site:** [🥽 AZ-305: Migration, HA & BCDR — Deep Dive](https://marcogrimaldi29.com/az-305-bcdr/)
> - ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)
> - 🔗 **Companion repos:** [📘 AZ-305 Study Notes](https://marcogrimaldi29.com/az-305-study-notes/) · [🥽 AZ-305: Azure Compute Services — Deep Dive](https://marcogrimaldi29.com/az-305-compute/) · [🥽 AZ-305: Azure Messaging Services — Deep Dive](https://marcogrimaldi29.com/az-305-messaging/) · [🥽 AZ-305: Data & Analytics Services — Deep Dive](https://marcogrimaldi29.com/az-305-data-analytics/) · [📘 AZ-104 Study Notes](https://marcogrimaldi29.com/az-104-study-notes/)

---

## 📋 Topics Covered

| Topic | Category | Key Exam Focus |
|-------|----------|---------------|
| 🏗️ **High Availability Design** | Architecture | HA vs DR, AZs, SLA composition, Traffic Manager, Front Door |
| 💾 **Azure Backup** | BCDR | Vault types, agents, soft delete, immutable vault, cross-region restore |
| 🔄 **Azure Site Recovery** | BCDR | Replication, Recovery Plans, RTO/RPO, failover types |
| 🔭 **Azure Migrate** | Migration | Migrate Hub, assessment, DMS, dependency analysis |
| 🌿 **Azure VMware Solution** | Hybrid Migration | SDDC, HCX live migration, connectivity, SKUs |
| 🗺️ **Migration Strategies** | Migration | 7 Rs, CAF phases, Landing Zones, tool selection |

---

## 🗂️ Repository Structure

```
az-305-bcdr/
├── README.md
├── index.md
├── 01-high-availability.md
├── 02-azure-backup.md
├── 03-azure-site-recovery.md
├── 04-azure-migrate.md
├── 05-azure-vmware-solution.md
├── 06-migration-strategies.md
├── 07-feature-comparison.md
└── 08-exam-caveats-cheatsheet.md
```

---

## 🌐 Published Website

This deep dive is hosted on **GitHub Pages** and published as a searchable website:

👉 **[🥽 AZ-305: Migration, HA & BCDR — Deep Dive](https://marcogrimaldi29.com/az-305-bcdr/)**

The site includes full-text search, Mermaid diagram rendering, and mobile-friendly navigation.

These notes are designed to be a structured, exam-focused summary of the most important concepts and services baseds on the official [Microsoft AZ-305 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-305) and its criteria.

Additional study notes maintained by me are also available for those pursuing Microsoft and Azure certifications at the following Landing Page:

👉 **[🛬 Landing Page: Study Notes](https://marcogrimaldi29.com/study-notes/)**

---

## ✍️ About the Author

These notes are maintained by **[Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)** — Cloud Consultant, Language Trainer & Lifelong Learner.

📍 **Find more content at [🏠 marcogrimaldi29.com](https://marcogrimaldi29.com)**

> The website is continuously updated and based on my personal study notes and experiences. If you have any feedback, suggestions, or corrections, feel free to [reach out](https://marcogrimaldi29.com/contact/)!

---

## 📈 Analytics

This site uses **[Umami](https://umami.is/)** for privacy-friendly analytics.

---

## 🐞 Spotted a Mistake?

Azure changes fast, so if something here is wrong or out of date, please [report an issue](https://github.com/marcogrimaldi29/az-305-bcdr/issues). The [contributing guide](.github/CONTRIBUTING.md) explains what makes a report quick to fix and what's out of scope.

---

## 💚 Support

If these notes helped you prepare for AZ-305, there are a couple of ways to show it: ⭐ star this repo on GitHub so other candidates can find it, or 🤝 connect with me on LinkedIn.

<p>
  <a href="https://github.com/marcogrimaldi29/az-305-bcdr"><img src="https://img.shields.io/badge/Star_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="Star on GitHub" /></a>
  <a href="https://www.linkedin.com/in/marco-grimaldi29/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2EyLjA2MiAyLjA2MiAwIDAgMS0yLjA2My0yLjA2NSAyLjA2NCAyLjA2NCAwIDEgMSAyLjA2MyAyLjA2NXptMS43ODIgMTMuMDE5SDMuNTU1VjloMy41NjR2MTEuNDUyek0yMi4yMjUgMEgxLjc3MUMuNzkyIDAgMCAuNzc0IDAgMS43Mjl2MjAuNTQyQzAgMjMuMjI3Ljc5MiAyNCAxLjc3MSAyNGgyMC40NTFDMjMuMiAyNCAyNCAyMy4yMjcgMjQgMjIuMjcxVjEuNzI5QzI0IC43NzQgMjMuMiAwIDIyLjIyNSAweiIvPjwvc3ZnPg%3D%3D" alt="Connect on LinkedIn" /></a>
</p>

---

## © Credits & Acknowledgements

The **[Just the Docs](https://github.com/just-the-docs/just-the-docs)** theme is used for a clean, documentation-style layout. Licensed under [MIT](https://opensource.org/license/MIT).

Created with the help of AI. Model used: **[Claude Sonnet 4.6](https://www.anthropic.com/news/claude-sonnet-4-6)**. The content has been reviewed and edited by the author for accuracy and clarity, but may contain errors. Always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/azure/).

> *Not affiliated with or endorsed by Microsoft.*