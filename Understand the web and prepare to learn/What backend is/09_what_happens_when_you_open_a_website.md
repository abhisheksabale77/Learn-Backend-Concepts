# Lesson 9 — What Happens When You Open a Website?

This lesson ties together everything learned so far by tracing the **full journey** of a web request.

---

## The scenario

You type `www.amazon.in` in your browser and press Enter. What happens?

---

## Step-by-step journey

```
┌──────────┐     ┌──────┐     ┌────────────┐     ┌──────────┐     ┌──────────┐
│  You +   │────►│ DNS  │────►│  Internet   │────►│  Server  │────►│ Database │
│  Browser │     │      │     │             │     │ (Backend)│     │          │
│          │◄────│      │◄────│             │◄────│          │◄────│          │
└──────────┘     └──────┘     └────────────┘     └──────────┘     └──────────┘
```

| Step | What happens | Analogy |
|---|---|---|
| **1. You type the URL** | You type `www.amazon.in` and press Enter | You tell the taxi driver: "Take me to Amazon's shop" |
| **2. DNS Lookup** | Your browser asks a **DNS server**: "What's the address (IP) for amazon.in?" DNS is like a **phone book** — it converts names to numbers | You look up the shop's actual street address |
| **3. Browser finds the server** | DNS returns an **IP address** (e.g., `52.95.120.67`). Your browser now knows where to send the request | You now know the exact street address |
| **4. Browser sends a request** | Your browser (the **client**) sends an **HTTP request** to that IP address: "Give me the homepage" | You arrive at the shop and say: "Show me what you have" |
| **5. Server receives the request** | The **server** (backend) receives the request and processes it | The shopkeeper hears your order |
| **6. Server talks to the database** | The backend queries the **database** to get products, deals, recommendations | The shopkeeper checks the shelves and inventory |
| **7. Server builds a response** | The backend puts together the data (HTML page, images, product info) | The shopkeeper prepares your items |
| **8. Response travels back** | The server sends the **HTTP response** back through the internet to your browser | The shopkeeper hands you the items |
| **9. Browser displays the page** | Your browser (frontend) reads the response and **renders** the page — you see Amazon's homepage | You see what you got |

---

## The whole picture in one line

> **Browser → DNS → Server (Backend) → Database → Server → Browser**

---

## Why this matters for backend developers

As a backend developer, **steps 5, 6, and 7 are YOUR job**:
- Receive the request
- Get data from the database
- Build and send the response

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **DNS (Domain Name System)** | The internet's **phone book** — converts human-readable names (`amazon.in`) to machine-readable IP addresses (`52.95.120.67`) |
| **IP Address** | A unique number that identifies a computer on the internet (like a street address) |
| **HTTP Request** | The message the browser sends to the server asking for something |
| **HTTP Response** | The message the server sends back with the requested data |
| **Render** | When the browser reads the response and displays the visual page |

---

## Core takeaway

> When you open a website: your browser asks DNS for the server's address, sends a request, the backend processes it, queries the database, and sends a response back. The browser then displays the page. As a backend developer, you build the receive → process → respond part.
