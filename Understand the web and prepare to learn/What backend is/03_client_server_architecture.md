# Lesson 3 — Client-Server Architecture

## What it is

**Client-server architecture** is a simple idea:

- One computer **asks** for something → that's the **client**
- Another computer **answers** → that's the **server**

That's it. The entire internet is built on this pattern — someone asking, someone answering.

---

## Real-world analogy — Post Office

| Post Office | Client-Server |
|---|---|
| **You** write a letter and drop it at the post office | The **client** (your browser/app) sends a **request** |
| The **post office** carries it to the recipient | The **internet** carries the request to the server |
| The **recipient** reads your letter and writes a reply | The **server** receives the request, processes it, and prepares a **response** |
| The reply comes back to you through the post office | The response travels back to the **client** |

---

## How it works step by step

```
┌────────┐         request          ┌────────┐
│        │  ───────────────────►    │        │
│ CLIENT │                          │ SERVER │
│        │  ◄───────────────────    │        │
└────────┘         response         └────────┘
```

1. **Client** — any device or software that makes a request. Examples: your browser, a mobile app, even another server.
2. **Server** — a computer (or software on a computer) that listens for requests, processes them, and sends back responses.
3. The client **initiates** — it always asks first. The server **never** contacts the client unprompted (in this basic model).
4. The server can handle requests from **many clients** at the same time.

---

## Everyday examples

| You do this... | Client | Server |
|---|---|---|
| Open google.com in Chrome | Chrome browser | Google's server |
| Open Instagram app | Instagram app on your phone | Instagram's server |
| Search on YouTube | YouTube website | YouTube's server |

---

## Key rules of client-server

1. **The client always starts the conversation** — the server just waits and listens.
2. **Many clients, one server** — one server can serve thousands of clients simultaneously.
3. **They communicate using agreed-upon rules** — these rules are called a **protocol** (like HTTP).

---

## Common misconception

- ❌ "A server is a special type of hardware."
- ✅ A server is just **any computer running software that listens for and responds to requests**. Your own laptop can be a server if you run server software on it.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Client** | Any device or software that sends a request |
| **Server** | A computer or software that listens for requests and sends back responses |
| **Request** | The message a client sends to ask for something |
| **Response** | The message a server sends back as an answer |
| **Protocol** | Agreed-upon rules for how client and server communicate (e.g., HTTP) |

---

## Core takeaway

> The client **asks**, the server **answers**. The client always starts the conversation. A server is not special hardware — it's any computer running software that listens and responds.
