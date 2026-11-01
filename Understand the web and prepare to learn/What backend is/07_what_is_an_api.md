# Lesson 7 — What is an API?

## What it is

**API** stands for **Application Programming Interface**.

In simple words: an API is a **set of rules and entry points** that allows one software to talk to another software.

---

## Real-world analogy — Restaurant Menu

| Restaurant | API |
|---|---|
| You sit at a table. You **can't walk into the kitchen** and cook yourself. | Your app **can't directly access** the server's database or code. |
| The restaurant gives you a **menu** — a list of things you're allowed to order. | The API provides a list of **endpoints** — specific requests you're allowed to make. |
| You tell the waiter "I want item #5" | Your app sends a request to a specific API endpoint, like `/users/profile` |
| The kitchen prepares it and the waiter brings it to you | The server processes the request and sends back the response |
| You can't order something **not on the menu** | You can't make a request the API doesn't support |

---

## Why do APIs exist?

Without an API, every app would need to directly access the server's database and internal code. That would be:

- 🔓 **Insecure** — anyone could read or delete all data
- 🤯 **Chaotic** — no rules about what you can or can't do
- 🔗 **Tightly coupled** — if the server changes internally, everything breaks

An API creates a **controlled, organized boundary** — "here's what you can ask for, and here's how to ask."

---

## How it works

```
Mobile App  ──► /api/users/profile  ──►  Server processes  ──►  Response: { name: "Abhishek", email: "..." }
Web App     ──► /api/users/profile  ──►  Same server, same API  ──►  Same response
```

Both the mobile app and the web app use the **SAME API**. The backend developer builds the API once, and multiple frontends can use it.

---

## A real-world example — Inventory App API

| What you want to do | API Endpoint |
|---|---|
| Get all assets | `GET /api/assets` |
| Add a new asset | `POST /api/assets` |
| Update an asset | `PUT /api/assets/42` |
| Delete an asset | `DELETE /api/assets/42` |

> `GET`, `POST`, `PUT`, `DELETE` are HTTP methods — we'll learn them in detail later. For now, just notice that the API provides **specific doors** for specific actions.

---

## Common misconception

- ❌ "API is a technology or a tool you install."
- ✅ An API is a **concept** — a defined way for software to communicate. As a backend developer, you design and build APIs.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **API (Application Programming Interface)** | A set of rules and entry points that allows one software to talk to another |
| **Endpoint** | A specific URL/address in the API that handles a specific action |

---

## Core takeaway

> An API is like a **restaurant menu** — it defines what the client is allowed to ask for and how to ask. It keeps the system **secure, organized, and flexible**. Backend developers design and build APIs.
