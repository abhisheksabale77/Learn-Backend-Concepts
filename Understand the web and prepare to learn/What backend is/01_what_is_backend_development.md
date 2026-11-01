# Lesson 1 — What is Backend Development?

## What it is

When you use any app or website — ordering food, checking your bank balance, or posting on social media — there are **two sides** working together:

1. **The part you see and interact with** (buttons, forms, images on screen)
2. **The part you don't see** that does the real work behind the scenes — storing your data, checking your password, calculating your balance, deciding what to show you.

**Backend development** is the craft of building that invisible second part — the engine running behind the curtain.

---

## Why it exists

Imagine a restaurant:

| Restaurant | Software |
|---|---|
| The **dining area** — menus, tables, decor — is what customers see | That's the **frontend** |
| The **kitchen** — where chefs receive orders, cook food, store ingredients, and send plates out — is hidden from customers | That's the **backend** |

Without the kitchen, the dining area is just a pretty room with no food. Without the backend, a website is just a pretty page that can't actually *do* anything — no login, no saving data, no processing.

---

## How it works (simplified)

```
You (customer)  →  Waiter (internet)  →  Kitchen (backend)  →  Waiter  →  You get your food
```

1. You tap "Show my orders" on an app.
2. That request travels over the internet to a **server** (a computer always running, always listening).
3. The backend software on that server receives the request, understands what you want, looks up your orders in a **database** (a structured store of information), and prepares a response.
4. The response travels back to your app, which displays your orders.

The backend developer writes the logic that happens in step 3 — **receive, process, respond**.

---

## What a backend developer actually builds

- The rules for **who can access what** (authentication & authorization)
- The logic for **storing, retrieving, updating, and deleting data**
- The **connections** between the app and the database
- The **APIs** (defined entry points) that frontends and other systems use to communicate with the backend

---

## Common misconception

- ❌ "Backend is just databases."
- ✅ Backend **includes** working with databases, but it also involves writing business logic, handling security, managing performance, processing background tasks, and much more.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Server** | A computer that is always running and listening for requests |
| **Database** | A structured store where data is saved and retrieved |
| **API** | A defined entry point that other systems use to talk to the backend |

---

## Core takeaway

> The backend's job is a three-part cycle: **Receive a request → Process it → Send a response.**
