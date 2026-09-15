<h1 align="center">Mishuk Adhikari</h1>

<p align="center">
  <b>Lead Software Engineer</b> · Cloud platforms, backend systems and production agentic AI<br>
  Dhaka, Bangladesh
</p>

<p align="center">
  <a href="https://mishuk.me"><img src="https://img.shields.io/badge/Website-mishuk.me-0f172a?style=flat-square&logo=firefox-browser&logoColor=white"></a>
  <a href="https://linkedin.com/in/mishuk-adhikari"><img src="https://img.shields.io/badge/LinkedIn-mishuk--adhikari-0a66c2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="https://mishukadhikari.github.io/mishuk.github.io/"><img src="https://img.shields.io/badge/CV-2026-334155?style=flat-square&logo=readthedocs&logoColor=white"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/followers/MishukAdhikari?style=flat-square&logo=github&logoColor=white&label=followers&color=334155">
  <img src="https://img.shields.io/github/stars/MishukAdhikari?style=flat-square&logo=github&logoColor=white&label=stars&color=334155">
  <img src="https://img.shields.io/badge/Laravel%20Telescope-merged%20upstream-FF2D20?style=flat-square&logo=laravel&logoColor=white">
</p>

---

I lead engineering on [xCloud](https://xcloud.host), a multi-cloud hosting and server-management
platform running **100,000+ websites**. Provisioning across half a dozen providers, the public and
enterprise APIs, billing and subscription workflows, Linux operations, and the tooling the rest of
the team builds on.

For the last while, most of my interesting work has been **agents that touch production** — and the
engineering problem there is not the prompt. It is blast radius.

## Agents in production

Three systems, all live, all built on the same principle: an agent gets exactly as much authority
as its job requires, and every use of it is on the record.

| System | What it does | How it stays safe |
| --- | --- | --- |
| **Pro Engineer** | Slack-based support-engineering agent. Picks up a case, gathers evidence, and hands a developer a finished investigation instead of a ticket. | Read paths only; escalates to a human rather than acting. |
| **Agent Bridge** | Evidence layer for server-side investigation. Lets an agent reason about a live box without being able to change it. | Scoped, audited, structurally read-only — there is no mutation path to misuse. |
| **Craft Mishuk** | Billing investigation agent wired to production data and Stripe. Reconstructs what actually happened to an account. | Reads freely, changes nothing without a human approving the specific change. |

**How I build them**

- **Least authority, enforced at the boundary** — scoped tokens and endpoint-level authorization, not a system prompt asking nicely.
- **Read-only by construction** — if an agent should not write, the write path should not exist for it.
- **Human approval on state changes** — anything touching money or customer infrastructure stops for a person.
- **Audited tool calls** — every action attributable after the fact, because "the agent did it" is not an answer.
- **Grounded in real data** — investigations run against production systems, not a summary of them.
- **Provider-agnostic** — MCP and a routing layer over OpenRouter, OpenAI and Anthropic; no single-vendor lock-in.

## Platform engineering

| Project | What it is |
| --- | --- |
| **xCloud Platform** | Provisioning, APIs, billing, authentication, backups, domains, deployments and day-to-day infrastructure operations. |
| **xCloud CLI & Terminal** | Public and enterprise API tooling with provider-agnostic AI support built in. |
| **Laravel Telescope** | Slow-query detection, merged upstream, plus a companion documentation contribution. |

Also: multi-cloud provisioning abstractions, public/partner/enterprise API architecture with scoped
tokens and OpenAPI contracts, revenue-sensitive billing workflows, and Laravel/PHP upgrades across a
large managed hosting fleet.

## Stack

![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Symfony](https://img.shields.io/badge/Symfony-000000?style=flat-square&logo=symfony&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white)
![Vultr](https://img.shields.io/badge/Vultr-007BFC?style=flat-square&logo=vultr&logoColor=white)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white)
![Linode](https://img.shields.io/badge/Akamai-0096D6?style=flat-square&logo=akamai&logoColor=white)

---

<p align="center">
  <img src="https://streak-stats.demolab.com?user=MishukAdhikari&hide_border=true&theme=transparent&date_format=M%20j%5B%2C%20Y%5D" height="180">
</p>

<p align="center"><sub>
Most of what I build is private, so the repos below are a poor sample of the work.<br>
The <a href="https://mishukadhikari.github.io/mishuk.github.io/">CV</a> is the honest version.
</sub></p>
