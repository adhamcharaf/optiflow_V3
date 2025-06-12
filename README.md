# Optiflow – Stock ERP AI‑Powered (MVP)

> ERP léger de gestion de stock, prévu pour une itération MVP de 4 semaines.
> Basé sur Next.js 19, tRPC, Supabase et modèles LLM via Cursor Agent & Claude Code.

## Fonctionnalités clés

* **Inventaire temps réel** : CRUD stock (PostgreSQL + Realtime Supabase)
* **Auth & RBAC Supabase** : rôles *admin* / *operator*
* **Prévision IA** : scripts Claude Code (Python 3.12, Prophet, scikit‑learn)
* **UI réactive** : Next.js + shadcn/ui
* **Cron & Webhooks** : Edge Functions + Supabase Cron
* **Monitoring** : Supabase observability & Logflare

## Stack

| Layer | Tech                                           |
| ----- | ---------------------------------------------- |
| Front | Next.js 19, React, shadcn/ui, Tailwind         |
| API   | tRPC, Zod                                      |
| Data  | Supabase (PostgreSQL, Edge Functions, Storage) |
| IA    | Cursor Agent (GPT‑4o, Gemini 2.5), Claude Code |
| CI    | GitHub Actions (pnpm, lint, test)              |

## Démarrage rapide

```bash
git clone git@github.com:<user>/stock-erp-ai.git
cd stock-erp-ai
pnpm install
cp .env.example .env      # SUPABASE_URL & SUPABASE_ANON_KEY
pnpm dev                  # http://localhost:3000
```

## Scripts utiles

| Commande       | Rôle                    |
| -------------- | ----------------------- |
| `pnpm dev`     | serveur dev Next.js     |
| `pnpm lint`    | ESLint + Prettier       |
| `pnpm test`    | Vitest                  |
| `pnpm migrate` | Supabase CLI migrations |

## Workflow vibecoding

1. Tâche ➜ branche `feat/<slug>`
2. `pnpm test` + micro‑doc (`docs/`)
3. PR vers `dev` ➜ review ➜ merge ➜ `main`.

## Roadmap

Consulter `roadmap_optiflow_mvp.md` pour les phases 0‑5.

## Licence

© 2025 Adham Charafeddine – Tous droits réservés.
