## Erbo at your service <img src='https://qpluspicture.oss-cn-beijing.aliyuncs.com/6LjjQA/Hi.gif' alt='Hi' width="24"/> 

Software engineer. Systems background. Building weird useful things.

I currently work as an SDE II at AWS. Before that, I spent a lot of time in C/C++ land: HTTP internals, server I/O, startup performance, network performance, and backend security.

I like turning messy problems into concrete systems, rules, and tradeoffs.

---

## What I’m Building

I’m actively working on a few projects that sit somewhere between:

~~~text
systems engineering
personal data
AI-native workflows
location-based products
tiny compilers
~~~

### 🥔 [Potato / erbos-lang](https://github.com/shanerbo/erbos-lang)

A small systems programming language that reads more like English and compiles to native ARM64 code.

Potato uses `.ptt` files and is designed around:

- Native compilation
- No VM, interpreter, libc, or runtime dependency
- Type checking
- Move semantics
- RAII-style scoped cleanup
- Bounds checking
- Fast single-pass compilation
- A compiler written in C

Example:

~~~text
spark {
  name is "world"
  yell("hello {name}")

  through (i from 1 to 10 by 1) {
    i mod 3 eq 0 ?{
      yell("fizz")
    } nah {
      yell(i)
    }
  }
}
~~~

This is where I explore language design, compiler construction, memory safety, and the question:

> How much can a tiny systems language do before it becomes a big one?

---

### 🗺️ [Fleck Backend / EatJournals](https://github.com/shanerbo/EatJournals)

Fleck is a private, map-first memory archive.

The idea:

~~~text
save moments
anchor them to places
revisit them by map or date
share read-only access through mutual connections
~~~

This repo owns the backend, web app, database, storage, and infrastructure:

- Next.js App Router
- TypeScript
- Prisma + Neon Postgres
- Cloudflare R2 private media storage
- Clerk authentication
- Signed media reads
- REST API for web and mobile clients
- MapLibre map surface
- Vercel deployment
- Terraform-managed infrastructure

Fleck is not just a CRUD app with a map slapped on top. It has real product constraints: privacy, auth, media storage, GPS data, mobile uploads, infra, and operational correctness.

---

### 📱 [FleckMobile](https://github.com/shanerbo/FleckMobile)

The native mobile client for Fleck.

The mobile app focuses on:

- Native iOS UX
- Local photo selection
- GPS-backed memory capture
- Batch upload orchestration
- Mobile API integration
- TestFlight distribution
- Simulator and device validation

The split is intentional:

~~~text
backend = canonical contracts, auth, storage, data model
mobile = capture flow, local UX, upload reliability
~~~

I care about the full loop: not just building an API, but making the product actually usable from someone’s phone.

---

## Engineering Background

I’ve worked mostly around backend and infrastructure systems:

- Backend systems
- Cloud services
- C / C++
- Network programming
- HTTP internals
- Performance optimization
- Security-sensitive systems
- Infrastructure design
- Product engineering
- Mobile/backend API design

I care about latency, correctness, simplicity, and whether the thing survives contact with reality.

---

## Technical Interests

- Systems programming
- Compiler design
- Backend architecture
- Cloud infrastructure
- AI agents
- Personal data products
- Maps and location-based software
- Mobile/backend integration
- E-commerce decision systems
- Fitness and nutrition data systems

---

## How I Think

I like:

- First principles over cargo culting
- Clear verdicts over vague analysis
- Small MVPs over big roadmaps
- Real user decisions over demo features
- Data over vibes
- Simple systems before clever systems
- Product constraints before technology choices

A good product should answer:

~~~text
What decision does this help the user make?
What behavior does this make easier?
What data does this preserve, transform, or clarify?
~~~

---

## Outside Software

Outside software, I train for running and cycling.

I like endurance sports for the same reason I like systems work: feedback loops, constraints, compounding improvement, and brutally honest measurements.

---

## Current Theme

Right now I’m building around this intersection:

~~~text
systems engineering
AI-native workflows
personal data
location-based products
decision systems
~~~

Small, useful products. Clear constraints. Real users. Less fluff.

---

## Links

Website: [erbos.me](https://erbos.me)  
GitHub: [@shanerbo](https://github.com/shanerbo)
