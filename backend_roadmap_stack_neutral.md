# Backend Roadmap: Stack-Neutral Beginner to Advanced

A project-driven roadmap for learning backend engineering from scratch. It preserves the original roadmap's phased progression, recurring Inventory Management Backend project, checklists, milestones, and advanced topics—but delays committing to a programming language and framework until you understand the fundamentals and can compare options.

**Assumptions:** beginner, approximately 10–15 hours per week. Adjust the timeline to your pace.

**Technology rule:** Do not commit to a backend stack on day one. First learn what backend systems do, how the web works, and the basic shape of programming. Then compare a small number of language options, choose one, and stick with it long enough to build a real application.

**Indicative timeline:** about 14–20 months to explore advanced engineering at 10–15 hours per week. Entry-level job readiness may come much earlier; it depends on your skills, projects, interview preparation, and local hiring requirements—not a fixed month.

---

## How to use this roadmap

Tick `[x]` only when both are true:

1. You used the concept in an exercise or project, not just watched or read about it.
2. You can explain it in your own words without notes.

Suggested weekly routine:
- 3 build/practice sessions.
- 1 review session where you explain what you learned and revisit mistakes.
- Keep notes about bugs, decisions, and what you would improve.

Aim for **70% building and practice, 30% reading or watching** once you begin coding.

## The recurring project

Build one project and extend it phase by phase: an **Inventory Management Backend** for assets, categories, users, and stock movements. Do not restart it every phase. Revisit and improve the same codebase as your understanding grows.

Optional alternative with similar learning value: a trade journal and alerts service.

---

## Phase 0: Understand the web and prepare to learn (Weeks 1–2)

**Goal:** understand what backend development is before selecting a language or framework.

### Learn

**What backend is**
- [ ] What is software development?
- [ ] Frontend vs backend vs full stack
- [ ] Client-server architecture
- [ ] What is a server?
- [ ] What is a web application?
- [ ] Static vs dynamic applications
- [ ] What is an API?
- [ ] What is a database?
- [ ] What happens when you open a website?
- [ ] What does a backend do when a user creates, reads, updates, or deletes data?

**Basic tools and workflow**
- [ ] What is a terminal and why developers use one
- [ ] Navigate folders and files from a terminal
- [ ] What is an editor or IDE?
- [ ] What is version control and why it matters
- [ ] What are Git and GitHub/GitLab used for?
- [ ] What is documentation and why should projects have a README?

**Programming concepts before choosing a language**
- [ ] What is an instruction and an algorithm?
- [ ] Input, processing, output
- [ ] Variables and values (conceptually)
- [ ] Conditions and repetition (conceptually)
- [ ] Functions and reusable logic (conceptually)
- [ ] Data collections and records (conceptually)
- [ ] Errors and debugging (conceptually)

### Build / practise
- Draw the journey of a request from browser to server and back.
- Write pseudocode for adding, finding, updating, and deleting an inventory asset.
- Install an editor and Git; create a repository with a README explaining the project idea.

### Done when
- [ ] You can explain client, server, API, and database in your own words.
- [ ] You can trace a simple request-response journey.
- [ ] You understand why you need a programming language to implement the logic.

### Postpone
TCP details, memory management, concurrency, advanced Linux, frameworks, databases in depth, and system design.

---

## Phase 1: Compare stacks, choose one language, and learn programming (Weeks 3–8)

**Goal:** make an informed initial technology choice and gain enough programming skill to build small programs.

You cannot implement a real backend without a programming language. The point is to delay the choice until you understand the job—not to avoid choosing forever.

### Compare a small number of candidate stacks

Research two or three options, such as:
- [ ] JavaScript/TypeScript with a server-side runtime and a web framework
- [ ] Python with a web framework
- [ ] Java with a backend framework
- [ ] C# with a backend framework
- [ ] Go with a web framework or standard library

For each candidate:
- [ ] Read the official beginner tutorial.
- [ ] Check current job listings in your target region and role.
- [ ] Check whether the language fits your interests and existing skills.
- [ ] Try a small program using variables, conditions, loops, functions, and collections.
- [ ] Compare documentation, ecosystem, learning curve, and project fit.
- [ ] Choose one language for the next phases. Do not keep switching because another stack looks popular.

**Framework selection comes later:** first learn core programming in your chosen language. Choose a web framework when you are ready to build your first API.

### Learn programming fundamentals in your chosen language

- [ ] Variables and data types
- [ ] Operators and expressions
- [ ] Conditions and loops
- [ ] Functions, parameters, return values, and scope
- [ ] Lists/arrays, maps/dictionaries, and sets
- [ ] Strings and date handling
- [ ] Data structures: lists, maps, sets, and queues at a basic level
- [ ] Modules and packages
- [ ] Dependency and package management
- [ ] Exceptions and error handling
- [ ] File input/output
- [ ] Basic debugging
- [ ] Object-oriented programming where relevant
- [ ] Encapsulation, inheritance, and polymorphism
- [ ] Basic algorithms and Big O
- [ ] Synchronous vs asynchronous programming (introductory understanding)
- [ ] Git commits, branches, and README files

### Build
- A command-line to-do app that saves tasks to a file.
- A script that reads a CSV file and prints a summary.
- Push both to your repository with clear READMEs.

### Done when
- [ ] You can write a small program without copying a tutorial line by line.
- [ ] You can read and write files, handle invalid input, and debug errors.
- [ ] You can explain the main data structures and functions you used.
- [ ] You have selected one language and can explain why it suits your current goal.

### Postpone
Advanced concurrency, detailed stack/heap memory internals, microservices, and multiple languages.

---

## Phase 2: HTTP, your first API, and a relational database (Weeks 9–16)

**Goal:** build a working CRUD API backed by a database.

Now choose a web framework that fits the language you selected. Use its official tutorial. The framework is an implementation choice; the concepts below transfer across stacks.

### Learn HTTP and networking essentials

- [ ] HTTP request and response structure
- [ ] HTTP methods: GET, POST, PUT, PATCH, DELETE
- [ ] Headers, body, path parameters, and query parameters
- [ ] HTTP status codes
- [ ] JSON and serialization
- [ ] Content types and content negotiation
- [ ] Statelessness
- [ ] Idempotency and safe methods
- [ ] Request-response lifecycle
- [ ] HTTP vs HTTPS (concept)
- [ ] DNS and domain names (introductory)
- [ ] IP addresses and ports (introductory)
- [ ] Pagination and filtering

### Learn API development

- [ ] REST and resources
- [ ] CRUD operations
- [ ] Routes and endpoints
- [ ] Request handlers/controllers
- [ ] Request validation
- [ ] Business logic
- [ ] Service and repository layers (as needed)
- [ ] Middleware or equivalent request pipeline
- [ ] Error handling and consistent error responses
- [ ] API documentation (for example, OpenAPI if supported)
- [ ] API testing with an API client or command-line tool
- [ ] Basic logging
- [ ] Configuration and environment variables

### Learn relational databases and SQL

- [ ] DBMS and database types
- [ ] Relational vs NoSQL databases (concept only for now)
- [ ] Tables, rows, and columns
- [ ] Primary keys and foreign keys
- [ ] SQL: SELECT, INSERT, UPDATE, DELETE
- [ ] WHERE, ORDER BY, and GROUP BY
- [ ] SQL joins and subqueries
- [ ] Database relationships
- [ ] Normalization and denormalization
- [ ] Constraints and data integrity
- [ ] Indexes (basics)
- [ ] Transactions and ACID properties
- [ ] Schema migrations
- [ ] ORM vs raw SQL
- [ ] Connection pooling (basics)
- [ ] N+1 query problem
- [ ] Backup and recovery basics

**Database choice:** choose one relational database with good documentation and local development support. PostgreSQL is a strong general-purpose option, but the database concepts are more important than the brand at this stage.

### Build: Inventory v1
- [ ] Create, read, update, and delete endpoints for assets and categories.
- [ ] Database schema with foreign keys and constraints.
- [ ] Request validation and meaningful error responses.
- [ ] Pagination and filtering on the asset list.
- [ ] README with setup instructions and example requests.

### Practice
- [ ] Practise SQL queries on [PostgreSQL Exercises](https://pgexercises.com) if you choose PostgreSQL, or use equivalent exercises for your chosen relational database.

### Done when
- [ ] You can build a CRUD API with a relational schema from a blank project.
- [ ] You can explain why a response might be 400, 401, 403, 404, 409, or 422.
- [ ] Data remains after the application restarts.
- [ ] Someone can follow your README to run the project locally.

### Postpone
GraphQL, gRPC, deep NoSQL study, and microservices.

---

## Phase 3: Authentication, security, testing, and application design (Weeks 17–26)

**Goal:** make Inventory safer, easier to maintain, and testable.

### Authentication and authorization

- [ ] Authentication vs authorization
- [ ] User registration and login
- [ ] Password hashing and salting
- [ ] Cookies and sessions
- [ ] Token-based authentication
- [ ] JWT concepts (if suitable for your chosen design)
- [ ] Access and refresh tokens (if needed)
- [ ] Role-based access control (RBAC) and permissions
- [ ] Resource-level authorization
- [ ] Session expiration and revocation
- [ ] Password reset and account recovery
- [ ] CORS and same-origin policy
- [ ] OAuth 2.0 fundamentals (stretch)
- [ ] OpenID Connect basics (stretch)
- [ ] Multi-factor authentication (stretch)

### Backend security

- [ ] Input validation
- [ ] SQL injection
- [ ] Cross-site scripting (XSS) and where backend validation fits
- [ ] Cross-site request forgery (CSRF) and when protections apply
- [ ] Broken access control
- [ ] Secure cookies and HTTPS
- [ ] Correct CORS configuration
- [ ] Secrets and environment security
- [ ] Least privilege
- [ ] Rate limiting and abuse prevention
- [ ] Safe error responses
- [ ] Dependency vulnerability management
- [ ] OWASP API Security Top 10
- [ ] Security logging and audit trails

### Testing and debugging

- [ ] Unit testing
- [ ] Integration testing
- [ ] End-to-end API testing
- [ ] Test doubles, mocks, and stubs
- [ ] Test databases and fixtures
- [ ] Assertions and test coverage
- [ ] Error and exception debugging
- [ ] Structured logging
- [ ] API contract testing (introductory)
- [ ] CI test automation

### Application architecture and code quality

- [ ] Layered architecture
- [ ] MVC pattern (understand when relevant)
- [ ] Controllers/handlers, services, and repositories
- [ ] Separation of concerns
- [ ] Dependency injection (if supported by your framework)
- [ ] SOLID principles
- [ ] DRY, KISS, and YAGNI
- [ ] Configuration management
- [ ] DTOs and data mapping
- [ ] Monolith vs modular monolith
- [ ] Refactoring and readable code
- [ ] Design patterns fundamentals (after you have experienced code that needs refactoring)

### Build: Inventory v2
- [ ] User registration and login.
- [ ] Roles such as admin, staff, and viewer.
- [ ] Resource-level permissions: users can only perform authorized actions.
- [ ] Automated tests with a separate test database.
- [ ] CI runs the test suite on every push.
- [ ] Document the main architecture and security decisions.

### Done when
- [ ] Unauthorized users cannot access protected data or actions.
- [ ] Tests catch at least one deliberately introduced bug.
- [ ] Someone else can clone the repository, follow the instructions, and run the app.
- [ ] You can demonstrate a security flaw in a controlled local test and then fix it.

---

## Phase 4: Deployment and production basics (Weeks 27–34)

**Goal:** deploy a real backend and learn how to operate it.

### Learn deployment and operations

- [ ] Linux server administration
- [ ] Processes, files, permissions, and resource usage
- [ ] Environment configuration
- [ ] Build and release process
- [ ] Web servers and reverse proxies
- [ ] Nginx or an equivalent reverse proxy
- [ ] Cloud computing fundamentals
- [ ] Virtual machines vs containers
- [ ] IaaS, PaaS, and serverless
- [ ] DNS and domain names
- [ ] TLS certificates and HTTPS
- [ ] Firewall and port configuration
- [ ] CI/CD pipelines
- [ ] Database migrations during deployment
- [ ] Rollback strategies
- [ ] Secrets management
- [ ] Docker concepts: images, containers, volumes, and networks
- [ ] Container orchestration basics using Docker Compose or an equivalent local tool

### Build: Inventory v3
- [ ] Deploy to a real server or cloud service.
- [ ] Configure a domain and HTTPS.
- [ ] Put a reverse proxy in front of the application when appropriate.
- [ ] Automate tests and deployment through CI/CD.
- [ ] Document deployment, configuration, and rollback steps.
- [ ] Keep secrets out of source control.

### Done when
- [ ] Someone can open your URL and use the application.
- [ ] You can redeploy and roll back safely.
- [ ] You can debug “site not loading” by checking DNS, firewall, ports, process health, and logs in order.
- [ ] You understand how to protect configuration and production data.

---

## Phase 5: Performance, concurrency, caching, and background work (Weeks 35–46)

**Goal:** measure performance, handle work outside the request path, and understand concurrency.

### Concurrency and execution models

- [ ] Concurrency vs parallelism
- [ ] Memory basics: stack and heap
- [ ] Synchronous vs asynchronous programming
- [ ] Async/await or the equivalent in your chosen language
- [ ] Event loops where relevant
- [ ] Threads and worker pools
- [ ] CPU-bound vs I/O-bound tasks
- [ ] Race conditions and shared state

### Performance and caching

- [ ] Response time and throughput
- [ ] Profiling and bottlenecks
- [ ] Database query optimization
- [ ] Indexes and query plans
- [ ] Caching fundamentals
- [ ] In-memory caching
- [ ] Redis or an equivalent external cache (only when justified)
- [ ] Cache-aside and write-through patterns
- [ ] Cache expiration and invalidation
- [ ] HTTP caching basics
- [ ] CDN basics
- [ ] Compression and pagination
- [ ] Connection pools and resource limits

### Database concurrency

- [ ] Isolation levels and locking
- [ ] Race conditions, lost updates, and double-submit handling
- [ ] Transaction boundaries
- [ ] Document and key-value database concepts

### Background processing

- [ ] Background jobs
- [ ] Task queues
- [ ] Message brokers
- [ ] Publish-subscribe pattern
- [ ] Events and consumers
- [ ] Retries and exponential backoff
- [ ] Dead-letter queues
- [ ] Idempotent job processing
- [ ] Scheduled tasks and cron
- [ ] Eventual consistency basics

### Real-time communication

- [ ] Polling and long polling
- [ ] Server-Sent Events (SSE)
- [ ] WebSockets
- [ ] Persistent connections
- [ ] Real-time notifications
- [ ] Presence and connection management

### Other API features

- [ ] File uploads and downloads
- [ ] Webhooks and signature verification
- [ ] API versioning
- [ ] API contract testing

### Build: Inventory v4
- [ ] Add search, filtering, and pagination.
- [ ] Seed a large dataset and measure query performance.
- [ ] Fix one slow query and record before/after results.
- [ ] Add a cache only if you can identify a real use case.
- [ ] Add a background low-stock alert with retries.
- [ ] Process CSV imports as background work.
- [ ] Add live stock updates using WebSockets or SSE if useful.
- [ ] Reproduce a race condition in stock updates and fix it.

### Done when
- [ ] You can show measured improvement to a slow query or endpoint.
- [ ] You can explain what happens if a background job runs twice.
- [ ] You understand the consistency and failure trade-offs of the features you added.

---

## Phase 6: Reliability and production hardening (Weeks 47–54)

**Goal:** understand what the application is doing and practise recovering from failures.

### Monitoring and reliability

- [ ] Application logging
- [ ] Metrics and dashboards
- [ ] Distributed tracing introduction
- [ ] Health checks
- [ ] Observability fundamentals
- [ ] Error monitoring
- [ ] Uptime and availability
- [ ] SLA, SLO, and SLI concepts
- [ ] Timeouts and retries
- [ ] Graceful shutdown
- [ ] Incident investigation
- [ ] Backup and disaster recovery
- [ ] Capacity and resource limits

### Deeper security

- [ ] OWASP API Security Top 10 review
- [ ] Secure file uploads
- [ ] Dependency vulnerability management
- [ ] Security logging and audit trails
- [ ] Server-side request forgery (SSRF)
- [ ] Secrets management in practice
- [ ] Security patching and incident response basics

### Load testing

- [ ] Load testing fundamentals
- [ ] Define a realistic traffic pattern
- [ ] Measure latency, throughput, errors, and resource use
- [ ] Find and explain a bottleneck
- [ ] Avoid running load tests against systems you do not own or have permission to test

### Build: Inventory v5
- [ ] Add dashboards and alerts for errors and latency.
- [ ] Load-test your own application and document the bottleneck.
- [ ] Restore the database from a backup as a recovery drill.
- [ ] Write a runbook for three likely failures.
- [ ] Document known limits and recovery steps.

### Done when
- [ ] You can explain a measured capacity limit with evidence.
- [ ] You can identify a failure from logs and metrics.
- [ ] You have successfully tested a database restore.
- [ ] You have a written runbook for common failures.

---

## Phase 7: Advanced system design and distributed systems (Month 12–20+)

**Goal:** design systems, reason about trade-offs, and understand when advanced architecture is justified.

Learn this phase after you can build, test, secure, deploy, and monitor a complete backend. Advanced topics are not prerequisites for every backend job.

### System design and scalability

- [ ] Functional vs non-functional requirements
- [ ] Capacity estimation
- [ ] Horizontal vs vertical scaling
- [ ] Load balancing
- [ ] Stateless application scaling
- [ ] Database replication
- [ ] Database partitioning and sharding
- [ ] Consistency and availability trade-offs
- [ ] CAP theorem fundamentals
- [ ] Distributed transactions
- [ ] Circuit breakers and bulkheads
- [ ] Backpressure and graceful degradation
- [ ] High availability and fault tolerance
- [ ] Multi-region architecture concepts

### Distributed systems and architecture

- [ ] Monolith vs microservices—and when not to split
- [ ] Service-to-service communication
- [ ] API gateways
- [ ] Service discovery
- [ ] Event-driven architecture
- [ ] Message delivery guarantees
- [ ] Outbox pattern
- [ ] Saga pattern
- [ ] CQRS
- [ ] Event sourcing
- [ ] Domain-driven design fundamentals
- [ ] Distributed locking
- [ ] Distributed tracing
- [ ] Service mesh overview
- [ ] Clean architecture overview
- [ ] Design patterns fundamentals
- [ ] GraphQL and gRPC overview
- [ ] WebRTC overview

### Specialized topics (choose based on interests or job needs)

- [ ] Full-text search and search engines
- [ ] Object storage and signed URLs
- [ ] Data retention and lifecycle management
- [ ] Multi-tenant SaaS architecture
- [ ] Payments and webhook reliability
- [ ] Geospatial data
- [ ] Streaming data systems
- [ ] Graph databases
- [ ] Time-series databases
- [ ] Kubernetes basics
- [ ] Infrastructure as Code
- [ ] Serverless event processing

### Build: Inventory v6
- [ ] Identify a real requirement that could justify separating a component, such as notifications.
- [ ] If justified, split that component into a separate service connected by a message queue.
- [ ] Implement idempotent consumers and failure handling.
- [ ] Write a one-page design document explaining what changed, what became harder, and whether the split was worthwhile.
- [ ] Design two other systems on paper, such as a URL shortener and a chat application.
- [ ] Compare your designs with reputable published designs.

### Done when
- [ ] You can turn vague requirements into a system design.
- [ ] You can estimate load, select components, and defend trade-offs.
- [ ] You can explain the operational costs and failure modes of your architecture.
- [ ] You can connect a design decision to a problem you have actually encountered.

---

## Rules that keep you moving

1. **Build more than you consume.** Watching tutorials is not the same as developing skill.
2. **Learn, build, break it deliberately, and explain it in writing.**
3. **Choose one language, one framework, and one primary database for the core project.** Change only when there is a clear reason.
4. **Do not start with microservices or Kubernetes.**
5. **Do not postpone databases, security, testing, or deployment.**
6. **Write code yourself first.** Use AI to explain errors, review your code, suggest tests, and quiz you—not to replace your learning.
7. **Read other people's code.** After learning your framework, study a reputable open-source project using it.
8. **Expect debugging to be part of learning.** Debugging your own code is progress.
9. **Do not add Redis, queues, or other infrastructure just because a roadmap mentions them.** Understand the problem first.
10. **Start applying for roles when you have the required fundamentals and credible projects.** You do not need to finish the advanced phase.

## Useful resources

Start with language-neutral material, then use the official documentation for the language and framework you choose.

- [Backend Developer Roadmap — roadmap.sh](https://roadmap.sh/backend)
- [HTTP overview — MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview)
- [Client-server overview — MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Server-side/First_steps/Client-Server_overview)
- [OWASP API Security guidance](https://devguide.owasp.org/en/07-training-education/07-api-top-ten/)
- [Git documentation](https://git-scm.com/doc)
- [PostgreSQL Exercises](https://pgexercises.com) (if you choose PostgreSQL)
- [Designing Data-Intensive Applications](https://dataintensive.net/) by Martin Kleppmann (advanced phase)

When you choose a language, add its official beginner tutorial and the official documentation for the framework you select.

## Your first week

1. Learn what a client, server, API, and database are.
2. Draw the request-response cycle for a simple website.
3. Install an editor and Git.
4. Learn basic terminal navigation.
5. Write pseudocode for creating, reading, updating, and deleting an inventory asset.
6. Create a Git repository with a README describing the project.
7. Compare two or three candidate languages using official beginner tutorials and a few current job listings.
8. Choose one language for Phase 1; do not spend weeks endlessly comparing stacks.

Do not worry about frameworks, Redis, Docker, or microservices yet. Your immediate goal is to understand the job, then learn enough programming to build your first small program.
