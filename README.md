### Erbo at your service <img src='https://qpluspicture.oss-cn-beijing.aliyuncs.com/6LjjQA/Hi.gif' alt='Hi' width="24"/> 

Software engineer. Systems background. AI product builder.

I currently work as an SDE II at AWS. Before that, I worked heavily with C/C++ systems programming, including HTTP protocol handling, server I/O, startup optimization, network performance, and backend security.

My core strength is taking ambiguous technical problems and reducing them into concrete systems, rules, and tradeoffs.

---

## What I’m Building

I’m actively working on three projects that reflect the same theme:

~~~text
low-level systems thinking
+ product-oriented software
+ personal data
+ AI-native workflows
~~~

### [Potato / erbos-lang](https://github.com/shanerbo/erbos-lang)

A systems programming language that reads closer to English and compiles to native ARM64 code.

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

This project is where I explore language design, compiler construction, memory safety, and how far a small systems language can go without carrying a large runtime.

---

### [Fleck Backend / EatJournals](https://github.com/shanerbo/EatJournals)

Fleck is a private, map-first memory archive.

The product idea is simple:

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

The current product is invite-only private beta.

I care about Fleck because it is not just another CRUD app. It is a personal data product with real constraints: auth, privacy, media storage, mobile upload reliability, maps, infrastructure, and operational correctness.

---

### [FleckMobile](https://github.com/shanerbo/FleckMobile)

The native mobile client for Fleck.

The mobile app focuses on:

- Native iOS user experience
- Local photo selection
- GPS-backed memory capture
- Batch upload orchestration
- Mobile API integration
- TestFlight distribution
- Simulator and device validation

The backend API contract lives in the Fleck backend repo, while the mobile app owns the native capture and upload flow.

This split is intentional: backend contracts stay canonical, while mobile remains focused on the user-facing capture experience.

---

## Engineering Background

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

I care about latency, correctness, simplicity, and operational reality.

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

## Principles

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

## Outside Engineering

I train seriously for running and cycling.

- Half marathon: **1:42**
- Cycling FTP: **266W**
- RBC GranFondo: **3:32**

Endurance sports shape how I think about software: measure honestly, build feedback loops, remove waste, and compound small improvements over time.

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

I’m especially interested in small, useful products that combine structured domain logic with practical software engineering.

---

## Links

Website: [erbos.me](https://erbos.me)  
GitHub: [@shanerbo](https://github.com/shanerbo)
