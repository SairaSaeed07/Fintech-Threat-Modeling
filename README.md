# Secure Fintech Payment Application - Threat Modeling (OWASP Threat Dragon)

## Overview

This project demonstrates how Threat Modeling can be integrated into a Secure Software Development Lifecycle (SSDLC) using OWASP Threat Dragon and Jira.

The objective was to identify security threats affecting a Fintech payment system, document mitigations, and track remediation tasks in Jira.

---

## Architecture

The application consists of:

- Customer
- Fintech API Gateway
- Payment Processor
- Transaction Database

Data Flow

Customer
↓

API Gateway
↓

Payment Processor
↓

Transaction Database

---

## Methodology

Threat modeling methodology:

- STRIDE
- OWASP Threat Dragon
- Jira for security task management

---

## Threats Identified

### 1. Unauthorized Customer/API Impersonation

Category

Spoofing

Severity

High

Mitigations

- OAuth 2.0
- OpenID Connect
- JWT Validation
- Mutual TLS
- Multi-Factor Authentication
- API Rate Limiting

---

### 2. Payment Request Manipulation

Category

Tampering

Severity

Critical

Mitigations

- TLS 1.3
- HMAC/JWS
- Request Integrity Validation
- Server-side Validation

---

### 3. API Gateway Resource Exhaustion

Category

Denial of Service

Severity

Critical

Mitigations

- WAF
- Rate Limiting
- Request Throttling
- Auto Scaling
- Circuit Breakers
- DDoS Protection

---

### 4. Duplicate Payment / Replay Fraud

Category

Tampering

Severity

Critical

Mitigations

- Idempotency Keys
- Transaction Nonces
- Replay Protection
- Duplicate Detection
- Fraud Monitoring

---

## Jira Security Tasks

All mitigations were tracked in Jira.

Implemented tasks include:

- Implement replay protection for payment requests
- Prevent API Gateway Denial of Service attacks
- Protect payment requests against tampering
- Implement strong authentication for Fintech APIs

---

## Tools Used

- OWASP Threat Dragon
- Jira
- STRIDE Threat Modeling
- GitHub
- Secure SDLC

---

## Skills Demonstrated

- Threat Modeling
- Secure Design
- STRIDE Analysis
- API Security
- Payment Security
- DevSecOps
- Risk Assessment
- Security Documentation
- Jira Security Tracking

---

## Repository Contents

- Threat Dragon Model (.json)
- Threat Modeling Report (.pdf)
- Jira Tracking
- Architecture Diagram

---

## Author

Saira Saeed

Cybersecurity | DevSecOps | Threat Modeling
