
---
type: project
status: active

project: MOD-SA
full_name: MOD-SA Intelligent Student Affairs Chatbot
organization: King Mongkut's University of Technology Thonburi (KMUTT)

language:

- Thai
- English

owner:
created:
updated:

tags:

- project
- rag
- llm
- chatbot
- knowledge-base

---

# MOD-SA Knowledge Vault

> **Single Source of Truth for the MOD-SA Project**

---

# Overview

MOD-SA is an intelligent chatbot project developed for **King Mongkut's University of Technology Thonburi (KMUTT)**.

The chatbot uses **Large Language Models (LLMs)** together with **Retrieval-Augmented Generation (RAG)** to answer questions from:

- Prospective students
- Newly admitted students
- Current students
- Parents
- University staff

The primary objective is to provide accurate, up-to-date, and trustworthy information about student services while reducing the workload of university staff.

---

# Purpose of this Vault

This Obsidian vault is **NOT** the RAG database.

Instead, it is the project's **Knowledge Management System (KMS)**.

It serves as the authoritative source for collecting, organizing, reviewing, maintaining, and validating knowledge before that knowledge is transformed into data suitable for the RAG pipeline.

Think of this vault as the project's **single source of truth**.

---

# Project Goals

- Centralize all knowledge related to student services.
- Organize information into maintainable domains and topics.
- Track knowledge sources and verification status.
- Support collaborative editing.
- Preserve relationships between pieces of knowledge.
- Prepare structured information for RAG ingestion.
- Support long-term maintenance of the chatbot.

---

# Knowledge Architecture

```

Official Sources  
│  
▼  
Source Documents  
│  
▼  
Knowledge Articles  
│  
▼  
Topic Notes  
│  
▼  
Domain Notes  
│  
▼  
Journey Pages  
│  
▼  
Export Pipeline  
│  
▼  
Markdown  
▼  
Chunking  
▼  
Metadata  
▼  
JSON  
▼  
Vector Database  
▼  
MOD-SA Chatbot

```

---

# Vault Structure

```

MOD-SA Vault/

├── 00 Project/  
│  
├── 01 Domains/  
│  
├── 02 Topics/  
│  
├── 03 Knowledge/  
│  
├── 04 Journeys/  
│  
├── 05 Sources/  
│  
├── 06 Templates/  
│  
├── 07 Assets/  
│  
├── 08 Reviews/  
│  
├── 09 Archive/  
│  
└── README.md

```

---

# Organization Philosophy

The vault is organized using three different perspectives.

## 1. Domains

Domains represent **major areas of knowledge**.

Examples:

- Academic & Registration
- Finance
- Scholarships
- Student Life
- Housing
- Digital Services
- Student Services

Domains act as indexes (Maps of Content) rather than storing detailed information.

---

## 2. Topics

Topics divide a domain into manageable subjects.

Example

Academic & Registration

- Course Registration
- Add/Drop
- GPA
- Graduation
- Academic Calendar

Topics connect detailed knowledge articles together.

---

## 3. Knowledge Articles

Knowledge articles contain the actual information.

Examples

- How freshmen register courses
- Credit requirements
- Dormitory application process
- Scholarship eligibility

These articles become the primary source for the RAG pipeline.

---

# User Journey

Knowledge is also connected through user journeys.

Example:

Prospective Student

↓

Admission

↓

Accepted

↓

Pay Tuition

↓

Register Student

↓

Orientation

↓

First Semester

↓

Graduation

A single knowledge article may belong to multiple journeys.

---

# Sources of Knowledge

Knowledge should only originate from reliable sources.

Examples include:

- University regulations
- Official announcements
- Student Affairs
- Registrar Office
- Academic Calendar
- Official university websites
- Verified manuals
- Approved FAQs

Every knowledge article should reference its original source whenever possible.

---

# Bilingual Content

The chatbot primarily serves Thai users.

Knowledge should therefore:

- Preserve the original Thai wording.
- Include English translations where useful.
- Record common abbreviations.
- Record synonyms used by students.

Example

Thai

> ลงทะเบียนเรียน

English

> Course Registration

Synonyms

- ลงทะเบียน
- ลงวิชา
- Register Courses

---

# Knowledge Lifecycle

```

Collect

↓

Verify

↓

Organize

↓

Review

↓

Approve

↓

Export

↓

Chunk

↓

Embed

↓

Deploy

```

Knowledge should never be exported into the RAG database before being reviewed.

---

# Design Principles

The vault follows these principles:

- Single Source of Truth
- Source-first documentation
- Maintainability
- Reusability
- Traceability
- Minimal duplication
- Human-readable
- Machine-friendly

---

# Relationship Between Components

```

Project

└── Domain

```

  └── Topic

         └── Knowledge

                └── Source

```

```

Knowledge articles may belong to:

- multiple topics
- multiple domains
- multiple user journeys

through Obsidian backlinks.

---

# Future Expansion

The knowledge base is designed to support future capabilities, including:

- Personalized responses
- Integration with university systems
- Student-specific information
- Calendar integration
- Interactive academic advising
- Administrative workflows
- Agentic AI features

---

# Project Status

Current Phase

Knowledge Collection & Organization

Next Phase

Knowledge Validation

Future Phase

Automated RAG Pipeline

---

# Vision

Create a sustainable, maintainable, and trustworthy knowledge base that enables MOD-SA to provide accurate, explainable, and continuously evolving assistance to every KMUTT student, parent, and staff member.
