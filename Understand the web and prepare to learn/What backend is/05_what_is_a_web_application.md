# Lesson 5 — What is a Web Application?

## What it is

A **web application** (web app) is a program that:

1. Runs on a **server**
2. Users access through a **web browser** (Chrome, Firefox, etc.)
3. Doesn't need to be installed on the user's device

---

## Real-world analogy — Electricity

| Generator (installed app) | Electricity from power grid (web app) |
|---|---|
| You **buy and install** it at your home | You just **plug in** — the power plant does the work |
| It runs **on your machine** | The heavy work happens **somewhere else** (power station) |
| You need to **update/maintain** it yourself | The power company **maintains** everything |

A web app is like electricity from the grid — you don't install anything heavy. You just open your browser, and the application runs on a server somewhere else.

---

## Examples you already use

| Web Application | You access it via... | Runs on... |
|---|---|---|
| Gmail | Browser (gmail.com) | Google's servers |
| YouTube | Browser (youtube.com) | YouTube's servers |
| Google Docs | Browser (docs.google.com) | Google's servers |
| ChatGPT | Browser (chatgpt.com) | OpenAI's servers |

---

## Web app vs Mobile app vs Desktop app

| Type | Installed? | Runs where? | Example |
|---|---|---|---|
| **Web app** | No — opens in browser | Mostly on the server | Gmail in Chrome |
| **Mobile app** | Yes — downloaded from store | On your phone + server | Instagram app |
| **Desktop app** | Yes — installed on computer | On your computer | MS Word (offline) |

> Many mobile apps are actually just **frontends** that talk to the **same backend** as the web app. Instagram's app and Instagram's website both talk to the same servers.

---

## Where does backend fit in?

As a backend developer, you build the **server-side part** of web applications — the logic that receives requests, processes data, and sends responses.

```
User's Browser (frontend)  ←──internet──→  Your Code on Server (backend)
```

---

## Common misconception

- ❌ "A web app is just a website."
- ✅ A **website** is mostly static pages (like a brochure). A **web app** is interactive — users can log in, submit data, get personalized content. Gmail is a web app, not just a website.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Web application** | A program that runs on a server and is accessed through a browser — no installation needed |
| **Website** | Mostly static pages that display information (like a digital brochure) |

---

## Core takeaway

> A web application runs on a **server** and users access it through a **browser** without installing anything. As a backend developer, you build the server-side logic that powers these web apps.
