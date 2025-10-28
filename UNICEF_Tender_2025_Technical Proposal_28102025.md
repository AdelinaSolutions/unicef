# TECHNICAL PROPOSAL

AI-Enabled IVR System and Online Feedback Platform for UNICEF Ukraine

Prepared by: PE Andrii Naida & Adelina Solutions LLC
Date: 28/10/2025

1. Executive Summary

This proposal outlines a comprehensive solution to design, develop, secure and maintain a robust AI-powered
Interactive Voice Response (IVR) system to enhance UNICEF Ukraine’s existing “Say it as it is” feedback and
complaint mechanism. It blends advanced voice technology with human-centered safeguarding, ensuring every
voice—especially children’s voices—is safely heard and acted upon.

The solution will create a multi-channel, user-centric communication platform accessible via traditional
telephony (PSTN), VoIP, web, and mobile apps. Building on the current online platform already operated by our
team, this system ensures continuity of service, seamless data migration, and enhanced features without
operational disruption.

Leveraging advanced large language models (LLMs), speech recognition technologies, and real-time analytics,
the platform will deliver 24/7 availability, high scalability, and strict security compliance, supporting rural
populations and vulnerable groups. UNICEF will gain a fully integrated toolset to process and respond to high
volumes of feedback efficiently while reducing dependency on manual operations.

Key features: on-prem STT, LLM with anonymization, TTS, unified case management (voice + web), automatic
safeguarding escalation, dashboards, training, and 12-month maintenance.

Delivery model: FOP Andrii Naida (Lead Contractor) with Adelina Solutions LLC (AI & integration) and Adelina
Outsourcing LLC (24/7 operations & continuity).

2. Understanding of UNICEF’s Requirements

UNICEF needs an accessible, confidential, inclusive channel for feedback/complaints with real-time visibility,
safeguarding & GDPR compliance, and seamless integration with the current online platform.
Our approach: automate routine, escalate sensitive, speak empathetically, protect data, and keep people in
control.

3. System Architecture and Technologies

The proposed solution is based on a microservices architecture, containerized with Docker and orchestrated via
Kubernetes clusters.

Key features:

•  Hybrid Cloud Model: Multi-zone deployments ensuring 99.9% uptime and disaster recovery objectives

within 4 hours.

•  Voice Processing Layer: Handles inbound/outbound calls, transcription, and speech recognition.
•  AI Conversation Engine: LLM-powered, customized for UNICEF-specific terminology and complaint

workflows.
Integration Layer: Bi-directional synchronization with the “Say it as it is” platform.

•
•  Analytics & Monitoring: Prometheus, Grafana, and ELK Stack for system monitoring; Power BI/Tableau

for insights.

•  Security Layer: RBAC, MFA, AES-256 encryption, ISO 27001 and GDPR compliance.

PE Andrii Naida & Adelina Solutions LLC Partnership

Layer

Purpose

Technologies

Telephony Gateway

PSTN/SIP connection & routing

Asterisk / Kamailio / SIP

STT (On-Prem)

Anonymization

LLM Layer (API)

# TTS

Secure transcription on GPU

Whisper Large-v3 / NVIDIA Riva ASR

Redact PII before LLM

Custom NER/regex pipelines

Intent, routing, response

GPT-5 / Claude / Gemini

Natural, supportive voice

Azure Neural / ElevenLabs / Coqui

Case Management

Unified voice+web tickets

Django / PostgreSQL

Monitoring & Analytics

Trends, QA, audit

Grafana / Power BI

4. AI-Enabled IVR System

The AI-driven IVR enables natural, conversational voice interactions:

•

Intent and sentiment detection to route calls intelligently.

•  Automatic escalation of complex issues to human agents.

•

Support for 100+ concurrent calls with low latency.

•  Accurate recognition of Ukrainian, Russian, and dialects (Surzhyk).

•  Automated updates and case references for transparency.

PE Andrii Naida & Adelina Solutions LLC Partnership

5. Integration with Existing Platform

Adelina Solutions currently maintains the “Say it as it is” platform, providing unmatched knowledge for
seamless integration:

•  Unified database for all voice and web cases.

•  Real-time synchronization for consistent case management.

•

•

Single admin dashboard for UNICEF staff.

Future-proof API layer for new integrations (e.g., messaging apps).

6. Transcription and Search

•  High-accuracy automated transcription with manual correction.

•

•

Full-text search and filtering by user, topic, time, and sentiment.

Sentiment analytics to flag emergencies or dissatisfaction patterns.

•  Export capabilities in .txt, .csv, .pdf.

7. Security and Data Privacy

•  Encryption: TLS/SSL in transit, AES-256 at rest.

•  Access Controls: RBAC, least-privilege, 2FA for admins

•  DDoS Protection: Cloudflare/Azure protection.

•  Compliance: ISO 27001, GDPR standards, PSEA: anonymization, user rights, safeguarding by design

•  Audit Logs: Full activity logging for accountability, periodic reviews, pen-tests

•  AI Ethics: Explainability, human-in-the-loop, bias monitoring

8. Analytics and Reporting

•  Real-time dashboards with system health metrics.

•  Predictive analytics for demand forecasting.

•  Automated case categorization and sentiment tagging.

•  Configurable reporting templates for UNICEF stakeholders.

PE Andrii Naida & Adelina Solutions LLC Partnership

9. Scalability and Reliability

•  Horizontal scaling with Kubernetes clusters.

•

Load balancing for peak performance.

•  Redundant systems for regional outages.

•  CDN integration for low-latency web access.

Capability

Description

Kubernetes Orchestration

Horizontal scale, auto-healing

GPU Elasticity

Uptime Target

Failover

Backups

Dynamic STT capacity

99.9% SLA (monitoring & alerts)

Auto-routing to live operators

Hourly snapshots + offsite encrypted copies

Even during outages/emergencies, hotline continuity is maintained — every voice can still be heard.

10. Maintenance and Technical Support

•  24/7 monitoring and SLA-driven response times.

•  Regular updates and automated deployment pipelines.

•  Quarterly security audits and optimization reviews.

•  Continuous improvement of AI models.

Priority

SLA Response

Examples

P1 Critical

P2 High

P3 Medium

P4 Low

< 2h

< 6h

< 12h

< 48h

IVR outage / calls failing

STT degradation / high latency

Minor defects / UI issues

Cosmetic changes / suggestions

11. Training and Handover

•  Workshops: Hands-on training for administrators, operators, and IT staff.

•  Comprehensive Documentation: Manuals, FAQs, and workflow guides.

•  Knowledge Transfer: Full capability handover for UNICEF autonomy.

Module

Objective

Format

System Administration

Manage cases, roles, reports

Online workshop

Safeguarding & Escalation

Handle sensitive calls

Onsite (Kyiv)

Analytics & Monitoring

Maintenance & Updates

Use dashboards & KPIs

Online

Retraining, configs

Hybrid (online + docs)

PE Andrii Naida & Adelina Solutions LLC Partnership

12. Competitive Advantages

•  Proven Expertise: Existing “Say it as it is” development and support team.

•  Cutting-Edge AI: Integration of GPT-5, Claude 4, Gemini 2.5.

•  Cultural Context: Dialect and linguistic nuances of Ukraine supported.

•

Security-First: Alignment with UNICEF’s highest security standards.

•  Agile Delivery: Fast implementation with no quality compromise.

13. Deliverables and Timeline

Milestone

Deliverable

Inception Phase

Technical design, system architecture, risk strategy

Prototype Development

Functional prototype, sample voice flows

Calibration

Voice tuning, anonymization QA

Soft Launch (5–10%)

Controlled rollout

Training & Handover

User manuals, training sessions

Full Launch (100%)

Integrated system with IVR and platform features

Maintenance & Support

Ongoing bug fixes, optimization

Deadline

# 22 NOV 2025

# 28 DEC 2025

# 05 JAN 2026

# 08 JAN 2026

# 19 JAN 2026

# 31 JAN 2026

# 31 DEC 2026

PE Andrii Naida & Adelina Solutions LLC Partnership

22 NOV 2528 DEC 2505 JAN 2608 JAN 2619 JAN 2631 JAN 2631 DEC 26InceptionPrototypeCalibrationSoft LaunchFull LaunchTrainingMaintenance & Support

14. Project Team

Role

Expertise

Project Manager

AI/IVR project oversight, stakeholder communication.

Lead System Architect

High-level design, integration strategy, security compliance.

Microservices & DevOps Specialist  CI/CD pipelines, container orchestration, scalability.

AI/NLP Lead

LLM fine-tuning, complaint workflows, intent detection.

Speech Recognition Specialist

Dialect support, transcription accuracy.

Backend & Frontend Developers

IVR logic, platform integration, dashboard design.

QA|Prompt Engineers

Manual and automated testing, usability verification.

Trainer/Documentation Specialist  Training programs, manuals, knowledge transfer.

Support Specialists

Team CVs attached

24/7 monitoring, maintenance, incident resolution.

15. Requirements Traceability Matrix (RTM)

Requirement

Solution

Comment

Microservices, Docker/Kubernetes  Cloud-based microservices architecture  Scalable CI/CD via API

Language Models & NLP

GPT-5, Claude 4, Gemini 2.5

Flexible selection per use case

Accent & Dialect Support

Ukrainian, Russian, Surzhyk

Inclusive communication

Voice Routing

SIP/VoIP, low-latency

Integration with “Say it as it is”

API/Webhooks

Seamless escalation

Unified backend

Transcription

Security & Privacy

Monitoring

Analytics

16. Summary

Automated + manual correction

Flexible QA

# ISO 27001, GDPR, AES-256, MFA

Certified infrastructure

Prometheus, Grafana, ELK

SLA tracking, centralized logs

Power BI, Tableau

Rich visualization and reporting

The Adelina Solutions AI Virtual Agent Platform fully meets UNICEF’s requirements, offering:

•  Advanced multilingual ASR and NLP tuned for Ukrainian context.

•  High scalability, reliability, and security compliance.

•

•

Seamless integration with UNICEF’s online platform.

Flexible infrastructure for future growth.

Prepared by:

Oleg Miroshnychenko

Approved by:

Oleg Chornobryvtsev

Supervised by:

Andrii Naida

PE Andrii Naida & Adelina Solutions LLC Partnership
