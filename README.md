## Erbo at your service <img src='https://qpluspicture.oss-cn-beijing.aliyuncs.com/6LjjQA/Hi.gif' alt='Hi' width="24"/> 

**Software engineer. Systems background. Building weird useful things.**

I currently work as an **SDE II at AWS**. Before that, I spent a lot of time in **C/C++ systems programming**: HTTP internals, server I/O, startup performance, network performance, and backend security.

I like turning messy problems into **concrete systems, rules, and tradeoffs**.

> My bias: useful software should either make something easier, clarify something messy, or help someone make a better decision.

---

## 🧭 Current Direction

I’m building around the intersection of:

~~~text
systems engineering
AI-native workflows
personal data
location-based products
decision systems
tiny compilers
~~~

Small products. Clear constraints. Real users. Less fluff.

---

## 🚧 Active Projects

### 🥔 [Potato / erbos-lang](https://github.com/shanerbo/erbos-lang)

**A tiny systems programming language that reads more like English and compiles to native ARM64.**

Potato uses `.ptt` files and is designed around:

- **Native compilation**
- **No VM, no interpreter, no libc, no runtime dependency**
- **Type checking**
- **Move semantics**
- **RAII-style scoped cleanup**
- **Bounds checking**
- **Fast single-pass compilation**
- **Compiler written in C**

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

What I’m exploring here:

- **Compiler construction**
- **Language design**
- **Memory safety**
- **Native code generation**
- **How much a small language can do before it becomes a big one**

> Question behind the project:  
> **Can a systems language be low-level, readable, and small at the same time?**

---

### 🗺️ [Fleck](https://github.com/shanerbo/EatJournals)

**A private, map-first memory archive.**

Fleck started from an older **food journal / AI logging** idea, but the product has pivoted. The direction now is closer to:

~~~text
memo
+ geospatial context
+ private social graph
+ personal archive
~~~

The product loop:

~~~text
capture memories
anchor them to places
revisit them by map or date
share selectively through private connections
~~~

This repo currently carries the legacy `EatJournals` name, but the product direction is **Fleck**.

The backend/web repo owns:

- **Next.js App Router**
- **TypeScript**
- **Prisma + Neon Postgres**
- **Cloudflare R2 private media storage**
- **Clerk authentication**
- **Signed media reads**
- **REST API for web and mobile clients**
- **MapLibre map surface**
- **Vercel deployment**
- **Terraform-managed infrastructure**

Why it’s interesting:

Fleck is not just a CRUD app with a map. It has real product constraints:

- **Privacy**
- **Auth**
- **Media storage**
- **GPS data**
- **Mobile uploads**
- **Private sharing**
- **Infrastructure**
- **Operational correctness**

> Product thesis:  
> **Your memories should be browsable by place, time, and people — without turning into public social media.**

---

### 📱 [FleckMobile](https://github.com/shanerbo/FleckMobile)

**The native iOS app for Fleck.**

FleckMobile owns the phone-side experience:

- **Import GPS-backed flecks**
- **Browse memories by map, place, and date**
- **Switch between your own map and connected maps**
- **Accept private connection invites through universal links**
- **Pick local photos and run resumable import sessions**
- **Handle retry, resume, cleanup, diagnostics, and TestFlight builds**

Stack:

- **Expo SDK 54**
- **React Native 0.81**
- **TypeScript**
- **Expo Router**
- **Clerk**
- **Apple Maps via `react-native-maps`**
- **TanStack Query with persisted cache**
- **Sentry**
- **EAS Build + TestFlight**

The split is intentional:

~~~text
Fleck backend = canonical API, auth, storage, database, infra
FleckMobile = native capture, map UX, upload reliability, TestFlight release
~~~

I care about the full product loop: not just making an API work, but making memory capture reliable from someone’s phone.

---

## 🧱 Engineering Background

I’ve worked mostly around **backend and infrastructure systems**:

- **Backend systems**
- **Cloud services**
- **C / C++**
- **Network programming**
- **HTTP internals**
- **Performance optimization**
- **Security-sensitive systems**
- **Infrastructure design**
- **Product engineering**
- **Mobile/backend API design**

I care about:

~~~text
latency
correctness
simplicity
operational reality
~~~

Or more directly:

> Does the system work when it meets real users, real data, real failures, and real constraints?

---

## 🧠 Technical Interests

- **Systems programming**
- **Compiler design**
- **Backend architecture**
- **Cloud infrastructure**
- **AI agents**
- **Personal data products**
- **Maps and location-based software**
- **Mobile/backend integration**
- **E-commerce decision systems**
- **Fitness and nutrition data systems**

---

## ⚙️ How I Think

I prefer:

- **First principles** over cargo culting
- **Clear verdicts** over vague analysis
- **Small MVPs** over big roadmaps
- **Real user decisions** over demo features
- **Data** over vibes
- **Simple systems** before clever systems
- **Product constraints** before technology choices

A good product should answer:

~~~text
What decision does this help the user make?
What behavior does this make easier?
What data does this preserve, transform, or clarify?
~~~

---

## 🏃 Outside Software

Outside software, I train for **running and cycling**.

I like endurance sports for the same reason I like systems work:

~~~text
feedback loops
constraints
compounding improvement
brutally honest measurements
~~~

---

## 🔗 Links

**Website:** [erbos.me](https://erbos.me)  
**GitHub:** [@shanerbo](https://github.com/shanerbo)
