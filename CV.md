# BACKEND ENGINEERING INTERNSHIP CV - KWEKU ANNAN

---

## EXECUTIVE SUMMARY

Results-driven backend engineer with demonstrated expertise in **RESTful API development, database design, microservices architecture, and cloud deployment**. Proven track record of building production-grade backend systems using Python, Flask, FastAPI, and relational databases. Strong focus on clean architecture, scalability, and real-world application development. 

**Notable Achievement:** Contributed core features to **Sitelytics** (formerly Site Audit AI), a production-grade SaaS platform launched during HNG Internship that is now a live commercial product serving real customers at [sitelytics.app](https://sitelytics.app/).

Active contributor to **open-source NLP projects** with GhanaNLP community supporting African language advancement.

---

## TECHNICAL CORE COMPETENCIES

### Backend Development
- RESTful API Design & Development (Flask, FastAPI, Python)
- Microservices Architecture
- Authentication & Authorization (API Key, Session-based, Basic Auth, OAuth2)
- API Gateway Implementation
- Request validation & Error handling
- Async/Await patterns (asyncio, SQLAlchemy async)
- Natural Language Processing integration

### Databases & Storage
- Relational Databases: MySQL, PostgreSQL, SQLite, SQL (Advanced queries, schema design)
- NoSQL Databases: MongoDB
- Database Design & Normalization
- ORM: SQLAlchemy (sync & async)
- Redis (Caching, rate limiting)
- Query optimization & indexing

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
- HTTP Clients: Requests, httpx (async)
- Database Adapters: PyMySQL, asyncpg
- Document Processing: PyPDF2, python-docx

---

## PROFESSIONAL PROJECTS

### Sitelytics: Site Audit AI ⭐ **PRODUCTION SAAS PLATFORM**

**Repository:** `emerjent/sitelytics-be` | **Live Product:** [sitelytics.app](https://sitelytics.app/)  
**Status:** Production Ready with Active Users | **Role:** Core Contributor  
**Team Size:** 15+ developers | **HNG Internship:** Progressed to Commercial Product

#### Project Overview
Sitelytics is an intelligent website auditing platform that automatically analyzes websites for accessibility, SEO, and performance issues. Started as an HNG Internship project, it has evolved into a live SaaS product with paying customers.

#### Key Technical Contributions

**1. OAuth2 Apple Authentication**
- Designed and implemented Apple Sign-In integration for secure third-party authentication
- Implemented OAuth2 protocol flow with Apple's authentication service
- Enabled seamless social login experience for users
- Proper token handling and user session management

**2. Lead Management System Enhancement**
- Extended database schema for professional services integration
- Added `LeadSource` enum with `PRO_REQUEST` capability
- Implemented `request_id` field linking leads to professional requests
- Automated lead creation/update workflow when users request professional services
- Wrote comprehensive integration tests (191 lines) covering request → lead pipeline

**3. System Architecture & Implementation**
- Modern FastAPI backend with vertical slice architecture
- Async/Await database operations with SQLAlchemy async ORM
- Multi-phase background job pipeline orchestration (Celery workers)
- Complex task sequencing: discovery → selection → scraping → analysis → aggregation
- Real-time progress tracking with percentage-based status updates

#### Technology Stack
- **Backend:** Python 3.11+, FastAPI, SQLAlchemy async ORM
- **Database:** PostgreSQL with Alembic migrations
- **Task Queue:** Celery + RabbitMQ for background job processing
- **Features:** OAuth2 social auth, automated workflows, real-time job tracking
- **Testing:** Comprehensive integration & unit tests
- **Architecture:** Vertical slice pattern with feature-based organization

#### Scale & Impact
- Production system with real users and active subscriptions
- Handles complex multi-stage scanning workflows
- OAuth2 integration enabling frictionless user onboarding
- Demonstrates production-grade code quality and testing

---

## HNG INTERNSHIP PROJECTS

Completed during **HNG Backend Internship** with progressive complexity and real-world impact. Multiple projects evolved into production systems.

### Stage 0: Gender Classifier API (HNG-14)

**Repository:** `kweku-annan/gender-classifier-api`

- **Objective:** Build a gender classification API using external data services
- **Features:**
  - Real-time name gender classification via Genderize API
  - Confidence scoring (probability + sample size thresholds)
  - UTC timestamp generation on every request
  - Robust error handling with appropriate HTTP status codes
  - HTTP connection pooling for efficiency
  - CORS support for frontend integration
- **Technologies:** FastAPI, httpx (async), Pydantic validation
- **Key Learning:** External API integration, HTTP connection pooling, proper error handling patterns

### Stage 0: Dynamic Profile Endpoint

**Repository:** `kweku-annan/HNG-0_dynamic_profile_endpoint`

- **Objective:** Build a RESTful API endpoint returning profile information with external API integration
- **Features:**
  - User profile information endpoint (`/me`)
  - Dynamic UTC timestamp generation
  - External API integration (Cat Facts API)
  - Error handling for API failures and timeouts
  - Production-ready configuration with Gunicorn
- **Technologies:** Python, Flask, Requests library, Railway deployment
- **Key Learning:** External API integration patterns and error handling

### Stage 1: Data Persistence & API Design Assessment

**Repository:** `kweku-annan/Data-Persistence-API-Design-Assessment`

- **Objective:** Build a backend system integrating multiple external APIs with data persistence
- **Features:**
  - **Multi-API Integration:** Concurrent calls to Genderize, Agify, Nationalize APIs
  - **Data Classification:** Age group categorization and nationality selection logic
  - **Idempotency Handling:** Prevents duplicate profiles through database pre-checks
  - **Full CRUD Operations:** Create, retrieve, filter, and delete profiles
  - **Advanced Filtering:** By gender, country, age group with optimization
  - **Proper HTTP Semantics:** 201, 204, 400, 422, 502 status codes with appropriate responses
- **Architecture:**
  - Separation of concerns (routers, services, integrations, models, schemas)
  - Layer independence for testability and maintainability
  - Configuration management with environment variables
  - Async/await best practices with httpx for non-blocking I/O
  - Concurrent API calls using asyncio.gather
- **Technologies:** FastAPI, PostgreSQL, SQLAlchemy ORM, Pydantic, asyncpg (async)
- **Database:** Designed for 2,026+ profile records with complex filtering
- **Key Learning:** System architecture, async patterns, clean code organization, idempotency patterns

### Stage 1.5: String Analyzer RESTful API

**Repository:** `kweku-annan/HNG-1-string_analyzer_api`

- **Features:** String analysis with computed properties, persistent storage, filtering, natural language query processing
- **Technologies:** Python, Flask
- **Key Learning:** Data transformation and query patterns

### Stage 2: Country Currency & Exchange API

**Repository:** `kweku-annan/HNG-2-country_currency_and_exchange_api` | **Deployed:** Railway.app

- **Objective:** Build a comprehensive country data API with external integrations
- **Features:**
  - Complete CRUD operations on 250+ country records
  - Multi-parameter filtering (by region, currency code)
  - Dynamic sorting by estimated GDP calculations
  - External API integration (REST Countries, Exchange Rates APIs)
  - Image generation for data visualization and summaries
  - Status tracking & data refresh endpoints
  - Error handling for external API failures
- **Technologies:** Python 3.12, Flask, SQLAlchemy, MySQL, PyMySQL, Pillow, Gunicorn
- **Deployment:** Railway.app with Aiven.io managed MySQL database
- **Key Learning:** Large-scale data management, external API orchestration, visualization generation

### Stage 2: Intelligence Query Engine Assessment

**Repository:** `kweku-annan/Intelligence-Query-Engine-Assessment`

- **Objective:** Extend Stage 1 with advanced querying capabilities
- **Features:**
  - Advanced filtering & sorting with multiple parameters
  - Pagination implementation for large datasets (2,000+ records)
  - **Natural Language Search Engine:** Rule-based NL parser (no AI)
    - Gender detection from natural language
    - Age group and age range extraction
    - Country detection from ~60 country names
    - Ambiguous query handling
  - Complex query optimization
  - Database indexing for performance
- **Technologies:** FastAPI, PostgreSQL, SQLAlchemy async, asyncpg, UUID v7
- **Database:** 2,000+ profiles with optimized indexes
- **Key Learning:** Query optimization, pagination patterns, NL parsing without LLMs, database indexing strategies

### Stage 3: Document Analyzer (HNG-13)

**Repository:** `kweku-annan/document-analyzer`

- **Objective:** Build an intelligent document processing service
- **Features:**
  - **Document Upload:** Support for PDF and DOCX files (up to 5MB)
  - **Text Extraction:** Automatic text extraction from documents
  - **AI-Powered Analysis:**
    - Concise document summaries via OpenRouter LLM integration
    - Automatic document type detection (invoice, CV, report, letter, contract, receipt, form)
    - Smart metadata extraction (dates, amounts, names, vendors)
  - **RESTful API:** Clean and well-documented endpoints
  - **Database Storage:** Persistent document and analysis results
  - **Interactive Documentation:** Auto-generated Swagger UI
- **Architecture:**
  - File storage service with size validation
  - Text extraction service (PyPDF2 + python-docx)
  - AI analysis service via OpenRouter API
  - Async file handling
- **Technologies:** FastAPI, PostgreSQL, SQLAlchemy, PyPDF2, python-docx, OpenRouter API, httpx (async)
- **Key Learning:** Document processing pipelines, LLM API integration, file handling, storage management

### API Gateway for Distributed Notification System

**Repository:** `kweku-annan/api-gateway`

- **Objective:** Build entry point for microservices notification architecture
- **Features:**
  - API Key-based authentication & authorization
  - Request validation & security middleware
  - Rate limiting (100 req/min per API key)
  - Idempotency support with 24-hour TTL
  - RabbitMQ message queue integration
  - Redis caching & status tracking
  - Correlation ID tracking for distributed debugging
  - Health check endpoint
  - Error handling with standard responses
- **Architecture:** Multi-service coordination (Email, Push, User services)
- **Deployment:** Docker Compose with Railway.app
- **Technologies:** Python, Flask, RabbitMQ, Redis, Docker

### Wallet Service

**Repository:** `kweku-annan/wallet-service` (part of HNG internship ecosystem)

- Financial transaction backend service
- Part of larger microservices ecosystem
- Technologies: Python, Flask, database design for transactions

### JobSearchAI

**Repository:** `kweku-annan/JobSearchAI` (part of HNG internship ecosystem)

- AI-powered job search backend
- Integration with search and matching algorithms
- Technologies: Python, FastAPI, NLP/ML integration

---

## GhanaNLP OPEN-SOURCE CONTRIBUTIONS 🌍 **COMMUNITY IMPACT**

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
- ✅ Endpoint design and implementation
- ✅ Request/response handling & HTTP semantics
- ✅ Error handling & validation
- ✅ Rate limiting & idempotency
- ✅ Async request handling (FastAPI)
- ✅ OAuth2 authentication
- ✅ External API integration & orchestration

### Database Engineering
- ✅ Schema design & normalization
- ✅ Complex queries & filtering with optimization
- ✅ ORM usage (SQLAlchemy sync & async)
- ✅ Database migrations (Alembic)
- ✅ Query optimization & indexing
- ✅ Multiple database systems (PostgreSQL, MySQL, SQLite)

### Security & Authentication
- ✅ API Key authentication
- ✅ Session-based authentication
- ✅ Basic authentication
- ✅ OAuth2 / social authentication
- ✅ Input validation & sanitization

### Microservices & Async
- ✅ Service decoupling
- ✅ Message queuing (RabbitMQ)
- ✅ Background job processing (Celery)
- ✅ Async/Await patterns
- ✅ Concurrent operations (asyncio.gather)
- ✅ API Gateway patterns

### DevOps & Deployment
- ✅ Docker containerization & Compose
- ✅ Environment management
- ✅ Production deployment (Railway)
- ✅ CI/CD pipeline integration
- ✅ Configuration management

### Testing & Code Quality
- ✅ Integration testing
- ✅ Unit testing
- ✅ Test-driven development
- ✅ Separation of concerns
- ✅ Clean architecture principles

### Data & Document Processing
- ✅ Document parsing (PDF, DOCX)
- ✅ Text extraction & analysis
- ✅ Natural language processing
- ✅ Data transformation & enrichment
- ✅ LLM API integration

---

## COLLABORATION & TEAM EXPERIENCE

- **Sitelytics Production Team:** Collaborated with 15+ developers on commercial SaaS platform with active users
- **HNG Internship:** Worked with diverse team building multiple production systems
- **GhanaNLP Community:** Contributing to open-source projects in collaborative environment
- **Code Review & PR Process:** Experienced with peer review, feedback integration, and community contributions

---

## LEARNING PATHWAY & PROGRESSION

| Phase | Focus | Outcome |
|-------|-------|---------|
| **Foundation** | ALX System Engineering & Low-level Programming | C, Shell scripting mastery |
| **Backend Track** | ALX Backend modules | Python, storage systems, authentication |
| **HNG Stage 0-2** | Progressive API complexity | External APIs → multi-service systems |
| **HNG Stage 3+** | Document processing & LLM integration | Advanced data pipeline design |
| **Production** | Sitelytics contribution | OAuth2, async systems, 15+ team collaboration |
| **Open-Source** | GhanaNLP community | NLP infrastructure & data processing |

---

## PROFESSIONAL ATTRIBUTES

- **Production Experience:** Actively contributing to live SaaS platform with real customers
- **Code Quality:** Structured projects with clean architecture, comprehensive testing, clear documentation
- **Scalability:** Designed systems managing 250+ entities, 2,000+ profiles, complex async pipelines
- **System Design:** Multi-layer architecture, separation of concerns, dependency injection, layer independence
- **Integration Expertise:** External APIs, OAuth2, LLMs, message queues, database migrations
- **Team Collaboration:** 15+ developer teams, code review experience, community engagement
- **Learning Agility:** Mastered FastAPI, async SQLAlchemy, Celery, OAuth2, NLP integration, document processing

---

## KEY METRICS

| Metric | Value |
|--------|-------|
| **Production SaaS Systems** | 1 (Sitelytics with active users) |
| **Team Size Experience** | 15+ developers |
| **HNG Internship Stages Completed** | 3+ (Stage 0 → 3+) |
| **Backend Projects** | 8+ projects (production & open-source) |
| **Database Systems Mastered** | MySQL, PostgreSQL, MongoDB, Redis, SQLite |
| **API Endpoints Built** | 30+ RESTful endpoints |
| **Data Scale Managed** | 2,000+ profiles, 250+ country records |
| **Authentication Methods** | API Key, Session, Basic, OAuth2 |
| **External Integrations** | 10+ third-party APIs |
| **Document Formats Supported** | PDF, DOCX with AI analysis |
| **Deployment Platforms** | Railway.app, Docker, self-hosted |
| **Open-Source Contributions** | Active GhanaNLP contributor |

---

## GITHUB PRESENCE

- **Username:** kweku-annan
- **Primary Profile:** [github.com/kweku-annan](https://github.com/kweku-annan)
- **Active Organizations:** GhanaNLP (open-source)
- **Production Collaboration:** emerjent/sitelytics-be (live commercial platform)

---

## AVAILABILITY

- **Duration:** 3-month internship
- **Focus:** Backend engineering, API development, system design, async systems, OAuth implementation
- **Ready for:** Immediate production system contribution, team collaboration, complex feature development

---

## STANDOUT ACHIEVEMENTS FOR BACKEND ENGINEERING INTERNSHIP

✅ **Commercial Product Experience** - Live contributor to Sitelytics SaaS platform  
✅ **OAuth2 Implementation** - Apple Sign-In authentication on production system  
✅ **System Architecture** - Designed multi-layer, testable backends from scratch  
✅ **Async Mastery** - FastAPI, SQLAlchemy async, concurrent API calls, Celery task queues  
✅ **Database Design** - Complex schemas, normalization, indexing, query optimization  
✅ **API Design Excellence** - Proper HTTP semantics, error handling, validation patterns  
✅ **Integration Expertise** - External APIs, OAuth2, LLMs, RabbitMQ, microservices  
✅ **Progressive Complexity** - HNG Stage 0 → 3+ with increasing system complexity  
✅ **Production Deployment** - Railway, Docker, real users, live transactions  
✅ **Team Collaboration** - Proven ability to integrate into large development teams  
✅ **Clean Code** - Separation of concerns, testability, documentation, maintenance  
✅ **Open-Source Engagement** - Active GhanaNLP community contributor

---

**CV Generated:** June 2026  
**Last Updated:** Based on comprehensive GitHub contribution analysis  
**Verified Content:** All facts sourced from public GitHub repositories and verified contributions
