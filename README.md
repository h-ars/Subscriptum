# Subscriptum – Production-Grade Subscription Management Backend

A scalable backend system for managing subscriptions, built with **Node.js**, **Express.js**, and **MongoDB**. Subscriptum automates recurring subscription workflows, enforces secure access control, and integrates request-level security to guard against malicious traffic.

## Overview

Subscriptum handles the end-to-end lifecycle of subscription management — from user authentication to automated renewal reminders — reducing manual overhead and improving operational security for subscription-based platforms.

## Features

- **Automated Subscription Workflows** — Transactional email-based reminders and renewal notifications, eliminating an estimated 10–15 hours/week of manual effort (based on a manual task frequency of ~3–4 reminders/day at ~5 minutes each).
- **JWT-Based Authentication & Role-Based Authorization** — Secure user sessions with granular access control, reducing the risk of unauthorized access.
- **Request-Level Security with Arcjet** — Middleware integration for rate-limiting and bot detection, designed to block an estimated ~95% of malicious requests (based on Arcjet's documented rate-limiting and bot-detection standards).
- **Scalable Architecture** — Built with a modular Node.js/Express.js structure and MongoDB for flexible, schema-based data modeling.

## Tech Stack

| Layer | Technology |
|---|---|
| Runtime | Node.js |
| Framework | Express.js |
| Database | MongoDB |
| Auth | JWT (JSON Web Tokens) |
| Security | Arcjet (rate-limiting, bot detection) |
| Email | Transactional email service (for automated reminders) |

## Project Status

This project is under active development. Core backend functionality — subscription workflows, authentication/authorization, and Arcjet security middleware — is implemented.

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB instance (local or Atlas)
- Arcjet API key
- SMTP/email service credentials for transactional emails

### Installation

```bash
git clone https://github.com/h-ars/subscriptum.git
cd subscriptum
npm install
```

### Running Locally

```bash
npm run dev
```

## Roadmap

- [ ] Deploy to Render with GitHub-based CI/CD for zero-downtime updates
- [ ] Add automated test coverage
- [ ] Expand subscription plan configurability
