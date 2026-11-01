# Lesson 6 — Static vs Dynamic Applications

## What it means

| Type | Meaning |
|---|---|
| **Static** | The content is **pre-built and fixed**. Every user sees the **same thing**. The server just sends files as-is. |
| **Dynamic** | The content is **generated on the fly** based on who's asking, what they want, or what's in the database. Different users may see **different things**. |

---

## Real-world analogy

| Static | Dynamic |
|---|---|
| A **printed newspaper** 🗞️ — everyone gets the same copy, same content. Once printed, it doesn't change. | A **news app on your phone** 📱 — it shows you personalized news, updates in real-time, and your saved articles are different from mine. |

---

## How they work behind the scenes

**Static application:**
```
Browser requests page  →  Server finds the ready-made HTML file  →  Sends it back
                           (no processing, no database lookup)
```

**Dynamic application:**
```
Browser requests page  →  Server runs code  →  Checks database  →  Builds the page  →  Sends it back
                           (processing happens every time!)
```

---

## Examples

| Static | Dynamic |
|---|---|
| A personal portfolio site | Facebook feed (different for every user) |
| A company "About Us" page | Amazon product page (personalized recommendations, real-time stock) |
| A documentation site | Online banking (shows YOUR balance, YOUR transactions) |

---

## Why does this matter for backend developers?

- **Static sites** need very little backend work — just serve files.
- **Dynamic applications** need a backend developer to write the logic that processes requests, queries databases, and builds responses.

> As a backend developer, your main job is building **dynamic** applications. That's where the real logic lives.

---

## Common misconception

- ❌ "Dynamic means the page has animations and moving elements."
- ✅ Dynamic means the **content changes based on data** (user, database, time). A static site can have fancy animations and still be static. A plain-looking banking site is dynamic because it shows YOUR data.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **Static application** | Content is pre-built and the same for everyone — server just sends files |
| **Dynamic application** | Content is generated on the fly based on who's asking and what's in the database |

---

## Core takeaway

> **Static** = same content for everyone, no processing. **Dynamic** = content generated per request using code and database. Backend developers mainly build dynamic applications.
