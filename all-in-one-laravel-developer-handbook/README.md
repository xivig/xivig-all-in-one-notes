# All-in-One Laravel Developer Handbook & Tutorials

[![Laravel](https://img.shields.io/badge/Laravel-12%20%7C%2013-FF2D20?style=flat-square&logo=laravel&logoColor=white)](https://laravel.com/docs)
[![PHP](https://img.shields.io/badge/PHP-8.3%20%E2%80%93%208.5-777BB4?style=flat-square&logo=php&logoColor=white)](https://www.php.net/)
[![Chapters](https://img.shields.io/badge/Chapters-34%20Chapters%20(4%20Tracks)-0EA5E9?style=flat-square)](./index.html)
[![Verified Labs](https://img.shields.io/badge/Runnable%20PHP%20Labs-Verified-10B981?style=flat-square)](./run-all-examples.php)
[![Interactive Portal](https://img.shields.io/badge/Portal-Interactive%20Handbook-f59e0b?style=flat-square)](https://htmlpreview.github.io/?https://github.com/xivig/xivig-all-in-one-notes/blob/master/all-in-one-laravel-developer-handbook/index.html)

A unified, step-by-step **Laravel 12/13 Developer Handbook** uniting **PHP 8.3–8.5 & OOP Container Internals**, **Production Blade UI, Faker, Eloquent (including Polymorphic & Locking), Multi-Guard Auth**, **Livewire 4, Inertia 2, Echo/Reverb & Ecosystem Packages**, **Server Configs & Troubleshooting**, **Batch CMS Scaffolding**, and the **EliteBlog Pro CMS Capstone**.

> Open the interactive handbook anytime: 🌐 **[Launch Live ↗](https://htmlpreview.github.io/?https://github.com/xivig/xivig-all-in-one-notes/blob/master/all-in-one-laravel-developer-handbook/index.html)** · **[Local (`index.html`)](./index.html)** — includes Dark/Light theme, `/` live search, 4 track filters, progress tracker (`0 / 34`), copyable snippets, runnable PHP lab drawers, and a **15-question Interactive Mastery Quiz**.

---

## Repository Map

| Resource | Purpose |
| :--- | :--- |
| [`index.html`](./index.html) | Interactive single-file handbook portal (search `/`, dark/light mode, 4 track filters, 15-question quiz, 34 chapters) |
| [`CHEATSHEET.md`](./CHEATSHEET.md) | High-density daily reference for Artisan CLI, Faker, Blade, Eloquent, Composer/Vite, Multi-Auth & Deploy commands |
| [`GLOSSARY.md`](./GLOSSARY.md) | Concise A–Z engineering glossary covering Laravel 12/13, Multi-Auth Guards, Polymorphic Relations, Observability & PHP 8.3–8.5 |
| [`scripts/laravel_artisan_setup.sh`](./scripts/laravel_artisan_setup.sh) | Batch CMS scaffolder (`--dry-run` supported) creating layouts, role partials, form components & 7 `-mfs` domain models |
| [`run-all-examples.php`](./run-all-examples.php) | Automated syntax & runtime verifier for all standalone PHP labs across chapters |
| [`chapters/`](./chapters) | 19 structured step-by-step deep dive chapters across Tracks 1–3 |
| [`../laravel-html-tutorials/`](./laravel-html-tutorials/) | 15 standalone dedicated HTML production blueprints (Track 4) |
| [`../laravel-text-tutorials/`](./laravel-text-tutorials/) | 15 dependency-free ASCII/Markdown plaintext terminal playbooks |

---

## Curriculum Overview (34 Chapters across 4 Tracks)

### Track 1 — PHP 8.3–8.5 & OOP Architecture for Laravel
| # | Chapter | Core Topics & Patterns | Runnable Lab |
| :---: | :--- | :--- | :--- |
| 01 | [PHP 8 Syntax, Types & Strict Mode](./chapters/01-php-8-syntax-types-and-strict-mode/README.md) | `strict_types`, union/intersection types, `??` vs `?:`, nullsafe `?->`, named arguments, typed class constants | [`lab.php`](./chapters/01-php-8-syntax-types-and-strict-mode/lab.php) |
| 02 | [OOP, Inheritance, Magic Methods & Lifecycle](./chapters/02-oop-inheritance-magic-methods-and-lifecycle/README.md) | `use ... as Authenticatable`, multi-level inheritance, `static::` (LSB), `__get`/`__set`/`__isset`/`__callStatic`, `clone` | [`lab.php`](./chapters/02-oop-inheritance-magic-methods-and-lifecycle/lab.php) |
| 03 | [Interfaces, Traits, Visibility & Contracts](./chapters/03-interfaces-traits-visibility-and-contracts/README.md) | `SoftDeletes` & `bootTrait`, Filament `implements`, Contract+Trait pattern, Controller `ApiResponse` trait, `protected` vs `private` | [`lab.php`](./chapters/03-interfaces-traits-visibility-and-contracts/lab.php) |
| 04 | [Modern PHP 8.3–8.5: Enums, Attributes, Hooks & Pipe](./chapters/04-modern-php-83-to-85-enums-attributes-hooks-and-pipe/README.md) | Readonly DTOs, Backed Enums + `match`, Laravel 13 PHP Attributes, `#[Override]`, `json_validate`, 8.4 hooks, 8.5 pipe `\|>` | [`lab.php`](./chapters/04-modern-php-83-to-85-enums-attributes-hooks-and-pipe/lab.php) · [`8.4`](./chapters/04-modern-php-83-to-85-enums-attributes-hooks-and-pipe/lab-php84.php) · [`8.5`](./chapters/04-modern-php-83-to-85-enums-attributes-hooks-and-pipe/lab-php85.php) |
| 05 | [Closures, Exceptions, Arrays & Strings for Laravel](./chapters/05-closures-exceptions-arrays-and-strings-for-laravel/README.md) | `use ($var)`, `fn =>`, `try`/`catch`/`finally`, `bootstrap/app.php` exception hooks, `Arr::only`, `Str::slug` & regex | [`lab.php`](./chapters/05-closures-exceptions-arrays-and-strings-for-laravel/lab.php) |
| 06 | [Composer PSR-4, Container Auto-Wiring & Facades](./chapters/06-composer-psr4-container-autowiring-and-facades/README.md) | PSR-4 namespace loading, `extra.laravel` auto-discovery, Reflection auto-wiring DI, Facade `__callStatic` proxies | [`lab.php`](./chapters/06-composer-psr4-container-autowiring-and-facades/lab.php) |

### Track 2 — Laravel 12/13 Core Foundations, UI Kits & Multi-Auth
| # | Chapter | Core Topics & Demo Projects | Runnable Lab |
| :---: | :--- | :--- | :--- |
| 07 | [Laravel Installation, Structure & Starter Kits](./chapters/07-laravel-installation-structure-and-starter-kits/README.md) | Version support matrix, `laravel new`, React/Vue/Livewire/WorkOS starter kits, `bootstrap/app.php` request lifecycle, `composer run dev` | — |
| 08 | [Routing, Controllers, Middleware & Responses](./chapters/08-routing-controllers-middleware-and-responses/README.md) | **Demo Project 1 (Agency Site)**, `Route::controller`, `Route::resource`, verb map & spoofing, middleware aliases, JSON responses | — |
| 09 | [Blade Templates, Components & Vite](./chapters/09-blade-templates-components-and-vite/README.md) | XSS escaping, full Admin/Blog Blade Layouts & Partials kit, responsive sidebar JS drawer, `@aware`/`--view`/`--inline`/`Blade::directive`, Vite | — |
| 10 | [SQL, Migrations, Faker, Seeders & Eloquent CRUD](./chapters/10-migrations-eloquent-models-and-relationships/README.md) | **Demo Project 2 (DevBlog)**, SQL joins, **Faker** (`fake()`, `Sequence`, `->recycle()`), `morphMany`/`morphTo`, `chunkById()`, `lockForUpdate()`, N+1 lab | [`lab.php`](./chapters/10-migrations-eloquent-models-and-relationships/lab.php) |
| 11 | [Validation, Uploads, Policies, RBAC & Multi-Auth](./chapters/11-forms-validation-policies-and-auth-crud/README.md) | **Demo Project 3 (Task Manager)**, FormRequests, `Storage::download`, `TaskPolicy`, RBAC pivot schema, **Hardened `web` + `admin` Multi-Guard Auth** | — |
| 12 | [Overriding Packages, Service Providers & Config](./chapters/12-overriding-packages-service-providers-and-configuration/README.md) | `register()` vs `boot()`, `bind`/`singleton`/`scoped`, `vendor:publish`, extending bound implementations, `.env` vs `config()` caching safety | [`lab.php`](./chapters/12-overriding-packages-service-providers-and-configuration/lab.php) |

### Track 3 — Production Laravel Engineering & Full Ecosystem
| # | Chapter | Core Topics & Patterns | Runnable Lab |
| :---: | :--- | :--- | :--- |
| 13 | [REST APIs, Resources, Sanctum & HTTP Client](./chapters/13-rest-apis-resources-sanctum-and-http-client/README.md) | `install:api`, `AuthTokenController`, `JsonResource` + `whenLoaded()`, `RateLimiter::for()`, HMAC webhooks, `Http::retry()` & `Http::pool()` | — |
| 14 | [Mail, Notifications, Commands, Queues & `defer()`](./chapters/14-queues-jobs-events-caching-and-defer/README.md) | `defer()`, Markdown `WelcomeMail`, multi-channel `Notification`, custom Artisan commands, `ShouldQueue`, `Cache::remember`/`flexible`/`touch` | — |
| 15 | [Automated Testing with Pest & PHPUnit](./chapters/15-testing-with-pest-and-phpunit/README.md) | `RefreshDatabase` + SQLite `:memory:`, `actingAs()`, Policy HTTP tests, `Queue::fake()` / `Mail::fake()` / `Storage::fake()`, Pest-style runner lab | [`lab.php`](./chapters/15-testing-with-pest-and-phpunit/lab.php) |
| 16 | [Security, Nginx/cPanel, Sail, Observability & Deploy](./chapters/16-security-performance-and-production-deployment/README.md) | OWASP checklist, **Nginx** & **cPanel** server configs, `optimize`, GitHub Actions CI, Docker/**Sail**, **Horizon/Pulse/Telescope**, Octane & L13 AI SDK | — |
| 17 | [Troubleshooting Playbook & Official Docs](./chapters/17-troubleshooting-and-diagnostics/README.md) | Systematic debugging flow (`artisan about`, `route:list`, `pail`, `queue:failed`), 11 root-cause fixes & curated official Laravel 13/12 docs | — |
| 18 | [Clean Architecture, Scaffolder, Capstone CMS & Roadmap](./chapters/18-clean-architecture-cms-capstone-and-roadmap/README.md) | Feature Action/Service layers, `scripts/laravel_artisan_setup.sh`, **EliteBlog Pro CMS** architecture & 12-week roadmap | — |
| 19 | [Livewire 4, Inertia 2, Echo, i18n & Ecosystem Packages](./chapters/19-livewire-inertia-realtime-i18n-and-ecosystem/README.md) | Reactive **Livewire 4**, **Inertia 2** React/Vue `useForm`, **Reverb + Echo** private channels, Localization (`__()`), **Socialite**, **Cashier** & **Scout** | — |

### Track 4 — Production Blueprints & Full-Stack Walkthroughs
| # | Chapter | Core Topics & Implementation | Dedicated HTML Guide | Plaintext Terminal Guide |
| :---: | :--- | :--- | :--- | :--- |
| 20 | Project Creation, Installer & Setup | Composer installer, SQLite/MySQL configs, `.env` keys, Artisan server loop | [Module 01 Guide](./laravel-html-tutorials/01-create-laravel-project.html) | [01-create-laravel-project.txt](./laravel-text-tutorials/01-create-laravel-project.txt) |
| 21 | Full-Cycle Workflow & Command Playbook | Scaffolding lifecycle (`make:model -a`), seeders, Tinker REPL, Vite bundling | [Module 02 Guide](./laravel-html-tutorials/02-workflow-command-playbook.html) | [02-workflow-command-playbook.txt](./laravel-text-tutorials/02-workflow-command-playbook.txt) |
| 22 | Laravel 100 Pro Tips & Initial Env Setup | 100 pro architecture rules, `APP_KEY`, `storage:link`, DB migration sequence | [Module 03 Guide](./laravel-html-tutorials/03-laravel-100-tips.html) | [03-laravel-100-tips.txt](./laravel-text-tutorials/03-laravel-100-tips.txt) |
| 23 | Admin Multi-Auth Architecture (Fortify) | Dedicated Fortify/Jetstream `admin` guard, `Admin` model & custom login pipeline | [Module 04 Guide](./laravel-html-tutorials/04-admin-multi-auth-fortify.html) | [04-admin-multi-auth-fortify.txt](./laravel-text-tutorials/04-admin-multi-auth-fortify.txt) |
| 24 | Step-by-Step Admin Authentication & Dashboard | 16-step manual auth flow, controller redirects, session guard protection | [Module 05 Guide](./laravel-html-tutorials/05-admin-login-step-by-step.html) | [05-admin-login-step-by-step.txt](./laravel-text-tutorials/05-admin-login-step-by-step.txt) |
| 25 | Multi-Authentication Master System & OTP | Multi-guard architecture, cryptographic OTP delivery, session isolation, RBAC | [Module 06 Guide](./laravel-html-tutorials/06-multi-auth-master-system.html) | [06-multi-auth-master-system.txt](./laravel-text-tutorials/06-multi-auth-master-system.txt) |
| 26 | Dynamic Menu Builder & Recursive Admin CRUD | Nested parent/child hierarchy, recursive Blade rendering, drag/reorder CRUD | [Module 07 Guide](./laravel-html-tutorials/07-dynamic-menu-crud.html) | [07-dynamic-menu-crud.txt](./laravel-text-tutorials/07-dynamic-menu-crud.txt) |
| 27 | App Scaffolding, Breeze & Dynamic CMS | Breeze scaffolding, multi-layout architecture (admin, user, blog), CMS cache | [Module 08 Guide](./laravel-html-tutorials/08-scaffolding-breeze-cms.html) | [08-scaffolding-breeze-cms.txt](./laravel-text-tutorials/08-scaffolding-breeze-cms.txt) |
| 28 | Project QA, Security Audit & Deployment | Pre-production security audit, DB indexes, Nginx tuning, queue supervisor | [Module 09 Guide](./laravel-html-tutorials/09-qa-deployment-checklist.html) | [09-qa-deployment-checklist.txt](./laravel-text-tutorials/09-qa-deployment-checklist.txt) |
| 29 | Pure PHP Vector SVG Math CAPTCHA | Zero-dependency pure PHP vector SVG math challenge generation & honeypots | [Module 10 Guide](./laravel-html-tutorials/10-math-captcha-security.html) | [10-math-captcha-security.txt](./laravel-text-tutorials/10-math-captcha-security.txt) |
| 30 | Production Technical SEO & Schema Markup | OpenGraph, Twitter Cards, JSON-LD Schema (Article, Breadcrumbs), XML sitemap | [Module 11 Guide](./laravel-html-tutorials/11-seo-metadata-schema.html) | [11-seo-metadata-schema.txt](./laravel-text-tutorials/11-seo-metadata-schema.txt) |
| 31 | RESTful APIs, Sanctum & JsonResources | `install:api`, token abilities, JsonResource pagination, rate limiting & error schemas | [Module 12 Guide](./laravel-html-tutorials/12-restful-api-sanctum-resources.html) | [12-restful-api-sanctum-resources.txt](./laravel-text-tutorials/12-restful-api-sanctum-resources.txt) |
| 32 | Advanced Eloquent Relations, Locks & Trans. | Polymorphic relations, `DB::transaction()`, pessimistic locking, observers & N+1 | [Module 13 Guide](./laravel-html-tutorials/13-eloquent-relationships-transactions.html) | [13-eloquent-relationships-transactions.txt](./laravel-text-tutorials/13-eloquent-relationships-transactions.txt) |
| 33 | Queues, Asynchronous Jobs & Scheduling | Database/Redis queue drivers, queued jobs with retry policies, events & cron | [Module 14 Guide](./laravel-html-tutorials/14-queues-jobs-events-scheduling.html) | [14-queues-jobs-events-scheduling.txt](./laravel-text-tutorials/14-queues-jobs-events-scheduling.txt) |
| 34 | Secure File Uploads, Disks & AWS S3 Storage | Multi-disk configurations (public/s3), mime validation, signed URLs, media | [Module 15 Guide](./laravel-html-tutorials/15-file-storage-uploads-media.html) | [15-file-storage-uploads-media.txt](./laravel-text-tutorials/15-file-storage-uploads-media.txt) |

---

## Quickstart: Verify Standalone PHP Labs & Scaffolder

Ensure PHP **8.3+** is available, then run:

```bash
php run-all-examples.php
```

Every chapter lab runs cleanly with zero Composer dependencies (`lab-php84.php` and `lab-php85.php` run automatically on PHP 8.4/8.5 and skip cleanly on PHP 8.3).

To preview the CMS scaffolder against any target directory without writing files:

```bash
bash scripts/laravel_artisan_setup.sh --dry-run
```

