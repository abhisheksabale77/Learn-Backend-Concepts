# Lesson 10 — What Does a Backend Do When a User CRUDs Data?

## What this is about

Almost everything a user does in an app boils down to **four operations** on data:

| Operation | Meaning | Example |
|---|---|---|
| **C**reate | Add new data | Sign up, post a photo, add a product |
| **R**ead | View existing data | See your profile, browse products, view orders |
| **U**pdate | Change existing data | Edit your name, change a price, update stock |
| **D**elete | Remove data | Delete a post, remove an account, cancel an order |

These four are called **CRUD** — the bread and butter of backend development.

---

## Real-world analogy — A school register

| CRUD | Register Book | Backend |
|---|---|---|
| **Create** | Write a new student's name in the register | Backend receives data, **validates** it, and **inserts** a new record in the database |
| **Read** | Look up a student's attendance record | Backend receives request, **queries** the database, and **sends** the data back |
| **Update** | Correct a student's misspelled name | Backend receives the change, **validates** it, **updates** the record in the database |
| **Delete** | Remove a student who transferred out | Backend receives the request, **checks permission**, and **removes** the record |

---

## What the backend does at each step

Example: Inventory app managing products.

### CREATE — "Add a new product"

```
1. Client sends:    POST /api/products  { name: "Laptop", price: 50000, stock: 25 }
2. Backend:
   a. Receives the request
   b. Validates: Is the name provided? Is price a positive number?
   c. Checks: Is this user authorized to add products?
   d. Saves to database: INSERT INTO products (name, price, stock) VALUES ('Laptop', 50000, 25)
   e. Sends response: 201 Created — { id: 1, name: "Laptop", price: 50000, stock: 25 }
3. Client shows: "Product added successfully!"
```

### READ — "Show all products"

```
1. Client sends:    GET /api/products
2. Backend:
   a. Receives the request
   b. Queries database: SELECT * FROM products
   c. Sends response: 200 OK — [ { id: 1, name: "Laptop", ... }, { id: 2, name: "Mouse", ... } ]
3. Client shows: List of products
```

### UPDATE — "Change the price"

```
1. Client sends:    PUT /api/products/1  { price: 45000 }
2. Backend:
   a. Receives the request
   b. Validates: Is price a positive number?
   c. Checks: Does product with id 1 exist?
   d. Updates database: UPDATE products SET price = 45000 WHERE id = 1
   e. Sends response: 200 OK — { id: 1, name: "Laptop", price: 45000, stock: 25 }
3. Client shows: "Price updated!"
```

### DELETE — "Remove a product"

```
1. Client sends:    DELETE /api/products/1
2. Backend:
   a. Receives the request
   b. Checks: Is this user authorized to delete?
   c. Checks: Does product with id 1 exist?
   d. Deletes from database: DELETE FROM products WHERE id = 1
   e. Sends response: 200 OK — "Product deleted"
3. Client shows: "Product removed!"
```

---

## The pattern

Every CRUD operation follows the same backend pattern:

```
Receive request  →  Validate  →  Check permissions  →  Talk to database  →  Send response
```

> This pattern — **receive, validate, authorize, database, respond** — is what you'll write hundreds of times as a backend developer. This IS the job.

---

## Common misconception

- ❌ "The frontend does CRUD operations."
- ✅ The frontend **triggers** CRUD by sending requests. The backend **performs** the actual create, read, update, or delete on the database. The frontend just displays the result.

---

## Key terms introduced

| Term | Simple meaning |
|---|---|
| **CRUD** | The four basic data operations: **C**reate, **R**ead, **U**pdate, **D**elete |
| **Validate** | Check that the incoming data is correct and complete before processing |
| **Authorize** | Check that the user has permission to perform this action |

---

## Core takeaway

> Almost every user action maps to a CRUD operation. The backend's job for each one is: **receive the request → validate the data → check permissions → talk to the database → send a response**. This pattern is the foundation of backend development.
