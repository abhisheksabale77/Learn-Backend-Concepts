# Lesson 4 — What is a Server?

## What it is

A **server** is simply a **computer (or a program on a computer) that waits for requests and sends back responses**. That's all.

It's not magic. It's a regular computer with a special job — **to serve**.

---

## Real-world analogy — Shopkeeper

| Shopkeeper | Server |
|---|---|
| Sits in the shop **all day**, waiting for customers | A server runs **24/7**, waiting for requests |
| A customer walks in and asks for rice | A client sends a request: "give me this user's data" |
| The shopkeeper goes to the shelf, finds the rice, and hands it over | The server processes the request, fetches data, and sends a response |
| The shopkeeper can serve **many customers** one after another (or simultaneously) | A server handles **many clients** at the same time |
| If the shopkeeper goes home, nobody gets served | If the server shuts down, no one can access the app |

---

## Key characteristics of a server

| Property | Meaning |
|---|---|
| **Always running** | A server typically runs 24/7 so clients can reach it anytime |
| **Listens on a port** | It listens on a specific **port** number (like a door number on a building) |
| **Handles multiple clients** | It can receive and respond to many requests at the same time |
| **Runs server software** | What makes it a "server" is the **software** running on it, not the hardware |

---

## Your laptop can be a server!

```
Your laptop running server software   →   It IS a server (for now)
Your laptop without server software   →   It's just a regular computer
```

In real companies, servers run on powerful computers in **data centers** — large buildings full of computers with fast internet, backup power, and cooling. But while learning, your own laptop can act as a server.

---

## Two meanings of "server"

People use the word "server" to mean two things:

| Meaning | Example |
|---|---|
| **Hardware** — the physical computer | "We bought a new server for the data center" |
| **Software** — the program listening for requests | "Start the server" (means start the program) |

As a backend developer, you'll mostly deal with the **software** meaning — you'll write and run server programs.

---

## Common misconception

- ❌ "Servers are expensive, special machines only big companies have."
- ✅ Any computer can be a server. When you build your first backend app and run it on your laptop, your laptop becomes the server.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Server** | A computer or program that waits for requests and sends responses |
| **Port** | A door number on a computer where the server listens for requests |
| **Data center** | A large building full of powerful computers that run servers 24/7 |

---

## Core takeaway

> A server is not special hardware — it's any computer running **software that listens for requests and sends responses**. Your own laptop becomes a server the moment you run server software on it.
