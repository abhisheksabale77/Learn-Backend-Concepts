# Lesson 2 — Frontend vs Backend vs Full Stack

## What are these three terms?

Think of building a house:

| Role | House | Software |
|---|---|---|
| **Interior designer** | Designs what the residents see — paint, furniture, layout | **Frontend developer** — builds what the user sees and interacts with (buttons, pages, animations) |
| **Plumber & electrician** | Builds the hidden systems — water pipes, wiring, drainage | **Backend developer** — builds the hidden systems — servers, databases, business logic, APIs |
| **General contractor** | Does both — knows the visible design AND the hidden systems | **Full-stack developer** — works on both frontend and backend |

---

## Why the separation exists

Building everything as one person's job becomes overwhelming for large applications. Splitting the work lets specialists focus:

- **Frontend** specialists focus on making the app look good, feel fast, and be easy to use.
- **Backend** specialists focus on making the app store data correctly, stay secure, and handle thousands of users.
- **Full-stack** developers can work across both sides, which is useful in smaller teams.

---

## A concrete example

When you search for a product on Amazon:

1. **Frontend** — the search box, the layout of results, the product images, the "Add to Cart" button.
2. **Backend** — receiving your search query, finding matching products in the database, checking stock, calculating prices, sending results back.
3. The **frontend** then takes those results and displays them beautifully.

---

## Important note

> Frontend and backend are not two separate apps fighting each other. They are **two halves of the same system**, designed to work together.

---

## Summary table

| Aspect | Frontend | Backend |
|---|---|---|
| **What user sees?** | Yes | No |
| **Handles data storage?** | No | Yes |
| **Handles security & auth?** | Partially (UI side) | Yes (real enforcement) |
| **Runs where?** | User's browser or device | Server |
| **Example technologies** | HTML, CSS, JavaScript, React | Servers, databases, APIs |

---

## Core takeaway

> **Frontend** = what the user sees. **Backend** = the hidden engine. **Full-stack** = both. They work together as two halves of one system.
