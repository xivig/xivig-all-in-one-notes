# Laravel Plaintext Engineering Playbooks & Notes

> **Format:** Clean, dependency-free, high-density ASCII/Markdown plaintext guides designed for direct copy-pasting into terminal sessions, SSH shells, configuration files, and IDEs.

This folder contains the **15 Master Production Playbooks** in plain text format. Each module pairs 1:1 with an interactive, syntax-highlighted web view located in [`../laravel-html-tutorials/`](../laravel-html-tutorials/index.html).

---

## ðŸ“‘ Complete Module Index & Cross-Reference

| # | Playbook Title | File | Topics & Features | HTML Counterpart | Related Handbook Chapter |
|---|----------------|------|-------------------|------------------|--------------------------|
| **01** | Laravel Project Creation & Setup Guide | [`01-create-laravel-project.txt`](./01-create-laravel-project.txt) | Composer installer, SQLite/MySQL configs, `.env` keys, Artisan server loop | [`01-create-laravel-project.html`](../laravel-html-tutorials/01-create-laravel-project.html) | [Ch. 07 Installation & Starter Kits](../chapters/07-laravel-installation-structure-and-starter-kits/README.md) |
| **02** | Full-Cycle Workflow & Command Playbook | [`02-workflow-command-playbook.txt`](./02-workflow-command-playbook.txt) | Full lifecycle command stream: scaffolding, migrations, tinker, Vite, Git | [`02-workflow-command-playbook.html`](../laravel-html-tutorials/02-workflow-command-playbook.html) | [Cheatsheet Reference](../CHEATSHEET.md) |
| **03** | Laravel 100 Pro Tips & Initial Setup Masterclass | [`03-laravel-100-tips.txt`](./03-laravel-100-tips.txt) | 100 pro architecture rules, `APP_KEY`, `storage:link`, DB migration sequence | [`03-laravel-100-tips.html`](../laravel-html-tutorials/03-laravel-100-tips.html) | [Ch. 18 Clean Architecture](../chapters/18-clean-architecture-cms-capstone-and-roadmap/README.md) |
| **04** | Admin Multi-Auth (Fortify & Jetstream) | [`04-admin-multi-auth-fortify.txt`](./04-admin-multi-auth-fortify.txt) | Multi-guard Fortify setup, dedicated `admin` guard, `Admin` model & migration | [`04-admin-multi-auth-fortify.html`](../laravel-html-tutorials/04-admin-multi-auth-fortify.html) | [Ch. 11 Multi-Guard Auth & Policies](../chapters/11-forms-validation-policies-and-auth-crud/README.md) |
| **05** | Admin Login & Dashboard (16 Steps) | [`05-admin-login-step-by-step.txt`](./05-admin-login-step-by-step.txt) | Exact 16-step implementation for admin auth, controller redirects & session guard | [`05-admin-login-step-by-step.html`](../laravel-html-tutorials/05-admin-login-step-by-step.html) | [Ch. 11 Multi-Guard Auth & Policies](../chapters/11-forms-validation-policies-and-auth-crud/README.md) |
| **06** | Multi-Authentication Master System & OTP | [`06-multi-auth-master-system.txt`](./06-multi-auth-master-system.txt) | Enterprise multi-auth architecture, OTP verification, guard switches & session isolation | [`06-multi-auth-master-system.html`](../laravel-html-tutorials/06-multi-auth-master-system.html) | [Ch. 11 Multi-Guard Auth & Policies](../chapters/11-forms-validation-policies-and-auth-crud/README.md) |
| **07** | Dynamic Menu Builder & Admin CRUD | [`07-dynamic-menu-crud.txt`](./07-dynamic-menu-crud.txt) | Nested parent/child hierarchy, recursive Blade rendering, drag/reorder CRUD | [`07-dynamic-menu-crud.html`](../laravel-html-tutorials/07-dynamic-menu-crud.html) | [Ch. 09 Blade & Layouts](../chapters/09-blade-templates-components-and-vite/README.md) |
| **08** | App Scaffolding, Breeze & Dynamic CMS | [`08-scaffolding-breeze-cms.txt`](./08-scaffolding-breeze-cms.txt) | Breeze scaffolding, multi-layout architecture (admin, user, blog), CMS cache | [`08-scaffolding-breeze-cms.html`](../laravel-html-tutorials/08-scaffolding-breeze-cms.html) | [Ch. 18 CMS Scaffolder & Architecture](../chapters/18-clean-architecture-cms-capstone-and-roadmap/README.md) |
| **09** | Project QA, Architecture & Deployment Checklist | [`09-qa-deployment-checklist.txt`](./09-qa-deployment-checklist.txt) | Pre-production security audit, DB indexes, Nginx tuning, queue worker supervisor | [`09-qa-deployment-checklist.html`](../laravel-html-tutorials/09-qa-deployment-checklist.html) | [Ch. 16 Production & Security](../chapters/16-security-performance-and-production-deployment/README.md) |
| **10** | Secure Math CAPTCHA & Anti-Spam Defense | [`10-math-captcha-security.txt`](./10-math-captcha-security.txt) | Pure PHP vector SVG math CAPTCHA, session verification, honeypot fields | [`10-math-captcha-security.html`](../laravel-html-tutorials/10-math-captcha-security.html) | [Ch. 16 Security & Hardening](../chapters/16-security-performance-and-production-deployment/README.md) |
| **11** | Production Technical SEO & Schema Markup | [`11-seo-metadata-schema.txt`](./11-seo-metadata-schema.txt) | Dynamic OpenGraph, Twitter Cards, JSON-LD Schema (Article, Breadcrumbs), XML sitemap | [`11-seo-metadata-schema.html`](../laravel-html-tutorials/11-seo-metadata-schema.html) | [Ch. 09 Blade & SEO Views](../chapters/09-blade-templates-components-and-vite/README.md) |
| **12** | RESTful API Development & Sanctum Auth | [`12-restful-api-sanctum-resources.txt`](./12-restful-api-sanctum-resources.txt) | `install:api`, token abilities, JsonResource pagination, rate limiting & error schemas | [`12-restful-api-sanctum-resources.html`](../laravel-html-tutorials/12-restful-api-sanctum-resources.html) | [Ch. 13 REST APIs & Sanctum](../chapters/13-rest-apis-resources-sanctum-and-http-client/README.md) |
| **13** | Advanced Eloquent Relationships & Transactions | [`13-eloquent-relationships-transactions.txt`](./13-eloquent-relationships-transactions.txt) | Polymorphic relations, `DB::transaction()`, pessimistic locking, observers & N+1 fixes | [`13-eloquent-relationships-transactions.html`](../laravel-html-tutorials/13-eloquent-relationships-transactions.html) | [Ch. 10 Eloquent, Migrations & Faker](../chapters/10-migrations-eloquent-models-and-relationships/README.md) |
| **14** | Queues, Asynchronous Jobs & Task Scheduling | [`14-queues-jobs-events-scheduling.txt`](./14-queues-jobs-events-scheduling.txt) | Database/Redis queue drivers, queued jobs with retry policies, events & cron scheduler | [`14-queues-jobs-events-scheduling.html`](../laravel-html-tutorials/14-queues-jobs-events-scheduling.html) | [Ch. 14 Queues, Events & `defer()`](../chapters/14-queues-jobs-events-caching-and-defer/README.md) |
| **15** | Secure File Uploads, Disks & AWS S3 Storage | [`15-file-storage-uploads-media.txt`](./15-file-storage-uploads-media.txt) | Multi-disk configurations (public/s3), mime validation, signed URLs, image optimization | [`15-file-storage-uploads-media.html`](../laravel-html-tutorials/15-file-storage-uploads-media.html) | [Ch. 11 Uploads & Form Requests](../chapters/11-forms-validation-policies-and-auth-crud/README.md) |

---

## âš¡ Terminal Usage Tips

### 1. Instant Text Search via CLI
To quickly find an artisan command, code pattern, or configuration option across all 15 text playbooks:

```bash
# PowerShell
Get-ChildItem -Path *.txt | Select-String -Pattern "lockForUpdate"

# Linux / macOS / Git Bash
grep -rn "lockForUpdate" *.txt
```

### 2. Copy Code Directly to Clipboard
```powershell
# Windows PowerShell
Get-Content .\04-admin-multi-auth-fortify.txt | Set-Clipboard

# Linux / Git Bash
cat 04-admin-multi-auth-fortify.txt | pbcopy   # macOS
cat 04-admin-multi-auth-fortify.txt | xclip    # Linux
```

### 3. Open Interactive HTML Version
Every `.txt` file above has a matching styled HTML guide with syntax highlighting and instant copying:
- Open [`../laravel-html-tutorials/index.html`](../laravel-html-tutorials/index.html) in your browser.
- Or view the master curriculum map in [`../README.md`](../README.md).


