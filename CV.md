# BACKEND ENGINEERING INTERNSHIP CV - KWEKU ANNAN

---

## EXECUTIVE SUMMARY

Results-driven backend engineer with demonstrated expertise in **RESTful API development, database design, microservices architecture, and cloud deployment**. Proven track record of building production-grade backend systems using Python, Flask, FastAPI, and relational databases. Strong focus on clean architecture, scalability, and real-world application development. Active contributor to **open-source NLP and data science projects** with GhanaNLP community.

---

## TECHNICAL CORE COMPETENCIES

### Backend Development
- RESTful API Design & Development (Flask, FastAPI, Python)
- Microservices Architecture
- Authentication & Authorization (API Key, Session-based, Basic Auth)
- API Gateway Implementation
- Request validation & Error handling
- Async/Await patterns (asyncio, SQLAlchemy async)

### Databases & Storage
- Relational Databases: MySQL, PostgreSQL, SQL (Advanced queries, schema design)
- NoSQL Databases: MongoDB
- Database Design & Normalization
- ORM: SQLAlchemy (sync & async)
- Redis (Caching, rate limiting)

### Infrastructure & DevOps
- Containerization: Docker, Docker Compose
- Cloud Deployment: Railway.app
- Environment Configuration & Management
- CI/CD Pipelines
- Message Brokers: RabbitMQ, Celery

### Tools & Frameworks
- Web Frameworks: Flask, FastAPI
- Queue Systems: RabbitMQ, Celery
- Database Migrations: Alembic
- HTTP Clients: Requests library
- Database Adapters: PyMySQL, asyncpg

---

## PROFESSIONAL & OPEN-SOURCE PROJECTS

### 1. Site Audit AI Backend (Sitelytics) ⭐ **PRODUCTION SYSTEM**

**Repository:** `emerjent/sitelytics-be` | **Status:** Production Ready | **Role:** Core Contributor

- **Architecture:** Modern FastAPI backend with vertical slice architecture (features-based organization)
- **Key Contribution:** Database schema extension for lead management & hire-a-pro integrations
  - Extended `LeadSource` enum with `PRO_REQUEST` capability
  - Added `request_id` field to link leads with professional requests
  - Implemented automatic lead creation/update workflow when users request professional services
  - Wrote comprehensive integration tests (191 lines) for request → lead pipeline
- **Scale & Complexity:**
  - Async/Await database operations with SQLAlchemy async ORM
  - Multi-phase background job pipeline (Celery workers)
  - Complex task orchestration (discovery → selection → scraping → analysis → aggregation)
  - Real-time progress tracking with status percentages
- **Tech Stack:** Python 3.11+, FastAPI, SQLAlchemy async, PostgreSQL, Alembic (migrations), Celery, RabbitMQ
- **Key Features:**
  - Vertical slice feature architecture
  - Database migrations with Alembic
  - Async request handling
  - Background job processing with Celery
  - Error handling with fallback mechanisms
  - Comprehensive integration & unit testing
- **Contributors Team:** 15+ developers (collaborative environment)

### 2. Country Currency & Exchange API

**Repository:** `kweku-annan/HNG-2-country_currency_and_exchange_api` | **Status:** Production Deployed

- **Architecture:** Designed and implemented full RESTful API with complex filtering, sorting, and pagination
- **Database:** MySQL with SQLAlchemy ORM; implemented advanced schema for currency exchange calculations
- **Features Delivered:**
  - Complete CRUD operations on 250+ country records
  - Multi-parameter filtering (by region, currency)
  - Dynamic sorting by estimated GDP
  - External API integration (REST Countries, Exchange Rates)
  - Image generation for data visualization
  - Status tracking & data refresh endpoints
- **Deployment:** Hosted on Railway.app with Aiven.io managed MySQL
- **Technologies:** Python 3.12, Flask, SQLAlchemy, MySQL, PyMySQL, Pillow, Gunicorn

### 3. API Gateway for Distributed Notification System

**Repository:** `kweku-annan/api-gateway` | **Status:** Production Ready

- **Architecture:** Entry point for microservices notification system; designed to coordinate multiple backend services
- **Core Responsibilities:**
  - API Key-based authentication & authorization
  - Request validation & security middleware
  - Rate limiting implementation (100 req/min per API key)
  - Idempotency support for duplicate prevention
  - RabbitMQ message queue integration
  - Redis caching & status tracking
  - Correlation ID tracking for distributed debugging
- **Features:** Health checks, error handling, Docker support, CI/CD pipeline
- **Deployment:** Docker Compose, Railway.app
- **Technologies:** Python, Flask, RabbitMQ, Redis, Docker

### 4. Intelligence Query Engine Assessment

**Repository:** `kweku-annan/Intelligence-Query-Engine-Assessment` | **Status:** Complete

- **Scale:** Database seeded with 2,026 profiles
- **Features:**
  - Advanced filtering & sorting
  - Pagination implementation
  - Natural language search endpoint
  - Complex query processing
- **Technologies:** Python, Flask, Database optimization

### 5. String Analyzer RESTful API

**Repository:** `kweku-annan/HNG-1-string_analyzer_api` | **Status:** Complete

- **Scope:** RESTful Flask service with data persistence
- **Capabilities:**
  - String analysis with computed properties
  - Data storage & retrieval
  - Filtering operations
  - Natural language query processing
- **Technologies:** Python, Flask

### 6. GhanaNLP Open-Source Contributions 🌍 **COMMUNITY IMPACT**

**Organization:** `GhanaNLP` | **Status:** Active Contributor

- **Mission:** NLP research and dataset curation for languages spoken in Ghana
- **Key Projects in Ecosystem:**
  - **GhanaLLM** - LLM experimentation for Ghanaian languages
  - **Ghana-QA** - Question-Answer pair curation from Ghanaian content
  - **nkrane** - Machine translation with terminology-controlled translation
  - **akiti-translator** - Rule-based translator for English to local language
  - **GhanaNouns** - Lexicon extraction from Ghanaian news & research
  - **GhanaTopics** - Topic identification from Ghanaian news
  - **kasa** - English to Twi translation system
  - **ghanaian-nlp-datasets-models** - Dataset & model curation
- **Contribution Focus:** Backend infrastructure, data processing pipelines, API development
- **Impact:** Supporting NLP advancement for underrepresented African languages

---

## BACKEND ENGINEERING SKILLS DEMONSTRATED

### API Development
- Endpoint design and implementation ✓
- Request/response handling ✓
- HTTP status code management ✓
- Error handling & validation ✓
- Rate limiting ✓
- Idempotency ✓
- Async request handling (FastAPI) ✓

### Database Engineering
- Schema design & normalization ✓
- Complex queries & filtering ✓
- ORM usage (SQLAlchemy sync & async) ✓
- Database optimization ✓
- Database migrations (Alembic) ✓
- PostgreSQL & MySQL expertise ✓

### Security & Authentication
- API Key authentication ✓
- Session-based authentication ✓
- Basic authentication ✓
- Input validation ✓

### Microservices & Async
- Service decoupling ✓
- Message queuing (RabbitMQ) ✓
- Service communication ✓
- API Gateway patterns ✓
- Background job processing (Celery) ✓
- Async/Await patterns ✓

### DevOps
- Docker containerization ✓
- Environment management ✓
- Production deployment (Railway) ✓
- CI/CD pipeline integration ✓

### Testing & Code Quality
- Integration testing ✓
- Unit testing ✓
- Test-driven development ✓

---

## COLLABORATION & TEAM EXPERIENCE

- **Sitelytics Team:** Collaborated with 15+ developers on production-grade system
- **GhanaNLP Community:** Contributing to open-source projects in team environment
- **Code Review:** Experienced in pull requests, peer review, and community contributions

---

## LEARNING PATHWAY

- **Foundation:** ALX System Engineering & Low-level Programming (C, Shell)
- **Backend Track:** Progressive development through ALX Backend modules:
  - Backend Python fundamentals
  - Backend storage (MySQL Advanced, NoSQL, Redis)
  - User data & authentication systems
- **Professional Projects:** HNG Internship Tasks (Stages 0-14) with increasing complexity
- **Open-Source:** Active contributor to GhanaNLP community projects

---

## PROFESSIONAL ATTRIBUTES

- **Code Quality Focus:** Structured project organization, clear documentation, comprehensive testing
- **Scalability Mindset:** Designed systems handling 250+ data records, 2,000+ profiles, complex async pipelines
- **Production Readiness:** Deployed applications to production environments; experience with real-world systems
- **Integration Experience:** External API consumption, microservices coordination, message queue management
- **Community Engagement:** Contributing to open-source NLP projects; team collaboration experience
- **Learning Agility:** Mastered FastAPI, async SQLAlchemy, Celery, and modern Python backend patterns

---

## KEY METRICS

| Metric | Value |
|--------|-------|
| **Completed Backend Projects** | 6+ projects (production & community) |
| **Production Systems Contributed To** | 1+ (Sitelytics) |
| **Database Systems Mastered** | MySQL, PostgreSQL, MongoDB, Redis |
| **API Endpoints Implemented** | 20+ RESTful endpoints across projects |
| **Profile Records Managed** | 2,026+ |
| **Countries in Production API** | 250+ |
| **Open-Source Contributions** | Active GhanaNLP community contributor |
| **Team Collaboration** | 15+ developers (Sitelytics team) |
| **Deployment Platforms** | Railway.app, Docker, self-hosted |

---

## GITHUB PRESENCE

- **Username:** kweku-annan
- **Primary Profile:** [github.com/kweku-annan](https://github.com/kweku-annan)
- **Active Organizations:** GhanaNLP (open-source contributions)
- **Notable Collaboration:** emerjent/sitelytics-be (production system)

---

## AVAILABILITY

- **Duration:** 3-month internship
- **Focus:** Backend engineering, API development, database design, async systems
- **Ready for:** Immediate contribution to production systems, team collaboration

---

**CV Generated:** June 2026  
**Last Updated:** Based on GitHub contribution analysis  
**Verified Content:** All facts sourced from public GitHub repositories and verified contributions
