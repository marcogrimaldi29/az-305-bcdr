---
layout: home
title: AZ-305 Migration, HA & BCDR — Deep Dive
nav_order: 1
description: "AZ-305 Exam Prep — High Availability Design, Azure Backup, Site Recovery, Azure Migrate, AVS, and Migration Strategies: product overviews, RTO/RPO tables, decision trees, and exam caveats."
permalink: /
mermaid: true
---

# 🥽 AZ-305: Migration, HA & BCDR — Deep Dive
{: .no_toc }

**Study Notes & Exam Prep — 2026 Edition**
{: .fs-5 .fw-300 }

[![Deploy to GitHub Pages](https://github.com/marcogrimaldi29/az-305-bcdr/actions/workflows/pages.yml/badge.svg)](https://github.com/marcogrimaldi29/az-305-bcdr/actions/workflows/pages.yml)
[![Personal Hub](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)

[Start Studying →](/az-305-bcdr/01-high-availability/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[View on GitHub](https://github.com/marcogrimaldi29/az-305-bcdr){: .btn .fs-5 .mb-4 .mb-md-0 }

> - 🎯 **Purpose:** Deep-dive study notes covering High Availability, Backup, Disaster Recovery, and Migration for the **AZ-305: Designing Microsoft Azure Infrastructure Solutions** exam — including Azure VMware Solution for hybrid migration scenarios.
> - 📅 **Version:** 2026
> - ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)
> - 🌐 **Published:** [🥽 AZ-305: Migration, HA & BCDR — Deep Dive](https://marcogrimaldi29.com/az-305-bcdr/)
> - 🔗 **Companion repos:** [📘 AZ-305 Study Notes](https://marcogrimaldi29.com/az-305-study-notes/) · [🥽 AZ-305: Azure Compute Services — Deep Dive](https://marcogrimaldi29.com/az-305-compute/) · [🥽 AZ-305: Azure Messaging Services — Deep Dive](https://marcogrimaldi29.com/az-305-messaging/) · [🥽 AZ-305: Data & Analytics Services — Deep Dive](https://marcogrimaldi29.com/az-305-data-analytics/) · [📘 AZ-104 Study Notes](https://marcogrimaldi29.com/az-104-study-notes/)

---

## 🗺 What's in This Repository?

| File | Coverage |
|------|----------|
| [🏗️ 01 — High Availability Design](01-high-availability.md) | HA vs DR, region pairs, AZs, SLA composition, load balancing, global routing |
| [💾 02 — Azure Backup](02-azure-backup.md) | Recovery Services Vault, Backup Vault, agents, policies, soft delete, immutable vault |
| [🔄 03 — Azure Site Recovery](03-azure-site-recovery.md) | Replication scenarios, Recovery Plans, RTO/RPO, test failover, agents |
| [🔭 04 — Azure Migrate](04-azure-migrate.md) | Migrate Hub, discovery & assessment, DMS, appliance, dependency analysis |
| [🌿 05 — Azure VMware Solution](05-azure-vmware-solution.md) | AVS SDDC, HCX, connectivity, SKUs, stretched clusters, integration |
| [🗺️ 06 — Migration Strategies](06-migration-strategies.md) | The 7 Rs, CAF phases, Landing Zones, tool selection per workload |
| [📊 07 — Feature Comparison](07-feature-comparison.md) | HA vs DR, Backup vs ASR, migration tools, RTO/RPO spectrum |
| [🎯 08 — Exam Caveats & Cheatsheet](08-exam-caveats-cheatsheet.md) | Decision trees, exam traps, must-memorise numbers, final checklist |

---

## 🔑 Why Migration, HA & BCDR Matters for AZ-305

This domain is explicitly tested across **two exam skill areas** and touches every layer of Azure architecture design:

- **Design for High Availability (15–20%):** Region pairs, Availability Zones, redundant services, SLA composition, global load balancing
- **Design for Backup and Disaster Recovery (10–15%):** RTO/RPO targets, Backup vs Site Recovery selection, vault configuration, cross-region restore
- **Design Migrations (10–15%):** Migration strategy selection, Azure Migrate tooling, database migration, VMware workload migration via AVS or HCX

> ⚠️ **The most common exam trap in this domain:** Confusing **High Availability** (staying up during failures) with **Disaster Recovery** (recovering after a failure). HA is about eliminating single points of failure. DR is about restoring service when HA has already failed. These require different services, different RPO/RTO targets, and different cost profiles.

---

## ⚡ Quick Navigation

| I need to know… | Go to |
|-----------------|-------|
| HA vs DR — the key distinction | [01 — HA § HA vs DR](01-high-availability.md#ha-vs-dr) |
| Recovery Services Vault vs Backup Vault | [02 — Backup § Vault Types](02-azure-backup.md#vault-types) |
| ASR replication scenarios | [03 — ASR § Supported Scenarios](03-azure-site-recovery.md#supported-scenarios) |
| Azure Migrate tooling overview | [04 — Migrate § Migrate Hub](04-azure-migrate.md#azure-migrate-hub) |
| AVS connectivity options | [05 — AVS § Connectivity](05-azure-vmware-solution.md#connectivity) |
| 7 Rs migration strategies | [06 — Strategies § The 7 Rs](06-migration-strategies.md#the-7-rs) |
| Backup vs ASR — which to use | [07 — Comparison § Backup vs ASR](07-feature-comparison.md#backup-vs-asr) |
| All exam traps in one place | [08 — Exam Caveats](08-exam-caveats-cheatsheet.md) |

---

## ©️ Credits & Acknowledgements

The [Just the Docs](https://github.com/just-the-docs/just-the-docs) theme is used for a clean, documentation-style layout. Licensed under [MIT](https://opensource.org/license/MIT).

Created with the help of AI. Model used: [Claude Sonnet 4.6](https://www.anthropic.com/news/claude-sonnet-4-6). The content has been reviewed and edited by the author for accuracy and clarity, but may contain errors. Always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/azure/).

> *Not affiliated with or endorsed by Microsoft.*