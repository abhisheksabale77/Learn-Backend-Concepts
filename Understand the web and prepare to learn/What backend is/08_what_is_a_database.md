# Lesson 8 — What is a Database?

## What it is

A **database** is an organized collection of data that can be **stored, accessed, updated, and deleted** easily.

Without a database, all your app's data disappears the moment the server restarts. A database makes data **permanent** (persistent).

---

## Real-world analogy — Filing Cabinet

| Filing Cabinet | Database |
|---|---|
| Has **drawers** organized by category (employees, invoices, clients) | Has **tables** organized by type (users, products, orders) |
| Each drawer has **folders** with individual records | Each table has **rows** — one row per record |
| Each folder has **fields** — name, phone, address | Each row has **columns** — name, email, password |
| You can **add** a new folder, **find** an existing one, **update** details, or **remove** a folder | You can **Create, Read, Update, Delete** data — this is called **CRUD** |
| If the office burns down and there's no backup, data is lost | If the database crashes and there's no backup, data is lost |

---

## What does a database store?

For an app like Instagram:

| Table | What it stores |
|---|---|
| **Users** | Name, email, password, profile photo |
| **Posts** | Image URL, caption, timestamp, who posted it |
| **Comments** | Comment text, who wrote it, which post it's on |
| **Followers** | Who follows whom |

---

## Why can't we just use files?

| Text File | Database |
|---|---|
| Hard to **search** — scan the entire file | Fast **search** — designed for quick lookups |
| Hard to **update** one record without rewriting the whole file | Easy **update** — change just one record |
| No protection if two users edit at the **same time** | Handles **multiple users** safely |
| No rules about what data is valid | Can enforce **rules** (e.g., email must be unique) |

---

## The backend's relationship with the database

```
Client  ──►  Backend (your code)  ──►  Database
Client  ◄──  Backend (your code)  ◄──  Database
```

The client **never** talks to the database directly. The **backend** sits in the middle — it receives the request, talks to the database, and sends the result back.

> The API controls what the client can ask for. The backend then decides **how** to get that data from the database. The client has **zero direct access** to the database.

---

## Common misconception

- ❌ "Database and server are the same thing."
- ✅ The **server** runs your backend code. The **database** stores data. They are separate — often running on different computers in production.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Database** | An organized collection of data that can be stored, accessed, updated, and deleted |
| **Table** | A structured group of related data (like a drawer in a filing cabinet) |
| **Row** | A single record in a table (like one folder in a drawer) |
| **Column** | A specific field in a record (like name, email, phone) |
| **CRUD** | The four basic operations: **C**reate, **R**ead, **U**pdate, **D**elete |
| **Persistent** | Data that survives restarts — it's saved permanently |

---

## Core takeaway

> A database is an **organized, permanent store of data**. The backend talks to the database on behalf of the client. The client never accesses the database directly. The four basic data operations are **CRUD** — Create, Read, Update, Delete.
