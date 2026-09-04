# Drew Beyersdorf

I'm an operator at [Methodology](https://www.gomethodology.com), a food manufacturing company in San Francisco. I didn't come up through engineering — I came up through the work. Kitchens, floors, delivery routes, labor plans, closes. I learned software and AI architecture because the systems I needed didn't exist, and waiting for someone else to build them wasn't working. So I built them myself.

Everything below is real and running. Most of it is private because it runs an actual company — real menus, real labor, real deliveries. I'm happy to talk about any of it.

**[drewbeyersdorf.com →](https://drewbeyersdorf.com)**

---

## The day job, systematized

Food manufacturing runs on clipboards, tribal knowledge, and heroics. I know because I did it. Piece by piece, I've been replacing the parts I lived:

- **Weekly floor OS** — the operating rhythm for a production week: nine lanes, five physical closes, two labor ledgers. What used to live in people's heads now lives in a system that stages the week and reconciles what actually happened.
- **Internal ops platform** — FastAPI + Next.js + Dagster over Supabase. Letters review, RAG over company knowledge, labor planning, deliveries. One platform instead of a dozen spreadsheets.
- **Data engineering** — ETL pipelines and DuckDB transforms so the numbers the floor runs on are the same numbers the business runs on.
- **Delivery operations** — built tooling to audit a full week of delivery instructions across 860 stops. That used to be nobody's job because it was impossible to do by hand.
- **Medically Tailored Meals** — research and execution toward Medicare Advantage MTM. Food is medicine; manufacturing it well at scale is an operations problem, and it's one worth solving.

## The self-learning layer

The bigger piece: an AI operations layer that ingests company knowledge, trains on it, dispatches agents, checks their work against ground truth, and corrects itself. Five layers — ingestion, training, inference, evaluation, and a constitution enforced by infrastructure instead of prompts. Rules that outlive the builder.

It runs on a small fleet I put together myself:

| Machine | Job |
|---|---|
| **charlie** | GPU workhorse — RTX PRO 6000 96GB, Threadripper 9960X |
| **nerve** | Always-on orchestrator — M4 Mini, 10W, runs 24/7 |
| **muscle** | Storage + fallback — RTX 5090, 16TB |
| **omarchy** | My laptop, where I drive it all |

The fleet is managed through a command bus with zero inbound ports: machines poll an outbox, run only whitelisted commands, and commit results back to an inbox. Git history is the audit log. Nothing runs that wasn't pre-approved.

## How I work

- **Domain first.** I build for problems I've personally had. The spec is the scar tissue.
- **Self-taught, on purpose.** Engineering, ML, agent architecture — learned by building, at night, against real deadlines.
- **Use what you build.** I dogfood everything. If I won't run my week on it, it isn't done.
- **Auditable or it didn't happen.** If a system acts, there's a record. No magic, no black boxes.
- **Small fleet, real work.** You don't need a data center. You need the right loops running all the time.

## Where this goes

Software agents coordinate the operation today. The same control plane — the command bus, the evaluation loops, the constitution — is what robotic cells on the floor will answer to tomorrow. That's the long game: the best-run food manufacturing operation in the world, built by the person who worked the floor, not someone who visited it once.

---

<p align="center">
  <img src="https://streak-stats.demolab.com?user=drewbeyersdorf&theme=transparent&hide_border=true" alt="GitHub streak stats for drewbeyersdorf" height="165" />
</p>

---

<p align="center">
  <a href="https://x.com/drewbeyersdorf">X</a> ·
  <a href="https://linkedin.com/in/drewbeyersdorf">LinkedIn</a> ·
  <a href="https://drewbeyersdorf.com">drewbeyersdorf.com</a>
</p>

---
