# Gooday brain: start here

This folder is the single source of truth for Gooday. Master copy: private GitHub repo `justiindtran-dev/gooday-brain` (bots sync the project folder with it every run). Justin, his co-founder and every bot read it before they work and update it after. If something is true about the business, it lives here. Everything else (Notion, chats, Miro) is a copy or a working space.

Last reviewed: 22 Nov 2026.

**Notion copy (read-only, for phones and the co-founder):** [Gooday brain (start here)](https://app.notion.com/p/42014ab463ca81a3b502ef580d13a017)

## What's in it

| File | What it holds | Who updates it |
|---|---|---|
| [company.md](company.md) | Who we are, contacts, accounts, tools and links | Founders |
| [product.md](product.md) | The two SKUs, spec, gel rule, pack design status | Founders, Nutritionist and Procurement bots |
| [brand.md](brand.md) | Name, trade mark status, look and voice, backup names | Founders, Marketing bot |
| [claims.md](claims.md) | What we can and can't say in ads and on pack | Founders, Research bot |
| [customers-and-market.md](customers-and-market.md) | Who buys, market size, competitors | Research and Marketing bots |
| [marketing.md](marketing.md) | Ad test, angles, creators, landing pages | Marketing bot |
| [suppliers.md](suppliers.md) | Manufacturers shortlist, status of each, RFQ | Procurement bot |
| [formulation.md](formulation.md) | Competitor benchmark per serve, effective doses, recommended formula per SKU and format (proposal) | Nutritionist bot |
| [finance.md](finance.md) | Unit economics per format and supplier, margins, break-even, first-batch cash, launch budget vs spend | Finance bot |
| [legal.md](legal.md) | Paperwork register: registrations, licences, contracts, policies, import and labelling by phase, with cost EST, who and status | Legal & admin bot, founders |
| [decisions.md](decisions.md) | Decisions made (with date and why), and open decisions | Founders only decide; bots may propose |
| [changelog.md](changelog.md) | One line per change to this folder | Everyone |

Deep work stays where it already is, and these pages link to it:
- `../daily-bots/reports/` dated bot reports (one file per bot per day)
- `../market-research/` full research write-ups
- `../brand/` trade mark check
- `../gooday-launch/` designs, ads, landing pages, ad test tracker
- `../agency-call-prep/` agency notes

## Rules for everyone (humans and bots)

1. **Read before you work.** Start with this README, then the page for your topic, then `decisions.md`.
2. **Update after you work.** If you learned a fact that changes a page, edit that page. Don't just leave it in a report.
3. **One fact, one place.** Link to a fact instead of copying it. If two pages disagree, fix the wrong one.
4. **Date your facts.** Write "(22 Nov 2026)" next to anything that can go stale: prices, MOQs, follower counts, trade mark status.
5. **Mark estimates.** Write EST for anything not published or confirmed, and link the source for facts.
6. **Bots propose, founders decide.** A bot never moves an item from "Open" to "Decided" in `decisions.md`. It can add an open question.
7. **Log the change.** Add one line to `changelog.md`: date, who, which file, what changed.
8. **No secrets.** Never put passwords, bank details or API keys in this folder.

## How to edit

Markdown is plain text. `#` is a heading, `-` is a bullet, `**bold**`, `[text](link)`, and tables use `|`. Any text editor works. [Obsidian](https://obsidian.md) (free) gives a nice view on desktop and phone: open this folder as a "vault".
