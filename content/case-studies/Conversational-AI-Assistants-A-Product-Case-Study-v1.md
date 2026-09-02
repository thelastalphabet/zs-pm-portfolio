# Slide 1

Conversational AI Assistants: A Product Case Study

Transforming student support through conversational AI — from concept to deployment

---

# Slide 2

PROBLEM STATEMENT

The Challenge

70K

Monthly Support Inquiries

Roughly 1 inquiry for every 2 learners at WGU

60K

Monthly Applications

Processed by Admissions and Enrollment teams at WGU

40%

Night Owls

Active learners between late-night hours (9 pm- 1 am), when WGU staff aren't available

Students frequently get blocked by basic questions when support is unavailable, while support staff spend significant time answering repetitive inquiries—resulting in delayed progress for students and reduced capacity for personalized support.

---

# Slide 3

DISCOVERY

Research Insights

UX Research Findings

Chatbot ranked top 3 preferred channels alongside email and SMS

Students wanted AI as additional resource but needed human connection for complex issues

Students are frustrated due to a lack of 24×7 support

Market Context

42% of higher ed leaders prioritize AI for customer service (Grammarly 2025)

Chatbots evolving beyond Q&A to agentic capabilities

Data Analysis

10% of enrollment calls involve questions covered on website

21% of support inquiries are questions covered in Student Handbook

25-48% of assessment calls are simple how-to requests

Domain Expert Input

Reduce cost per new student start

Proactively detect and support struggling applicants

Enable real-time chat for instant answers

---

# Slide 4

Product Vision

We envision a learning experience where every learner is guided by an AI assistant that delivers instant support, anticipates their next step, and seamlessly connects them to human experts when it matters most.

A digital concierge—a conversational AI companion designed as a trusted guide throughout the entire student journey, from enrollment through graduation.

---

# Slide 5

HYPOTHESIS

Our Core Hypothesis

Personalization

AI assistant evolves from helpful guide to intelligent autonomous companion

Efficiency

Reduces staff reliance on routine inquiries, enabling focus on complex requests

Accessibility

Delivers instant support at every stage of student journey

Retention

Improved engagement drives better completion rates

---

# Slide 6

SUCCESS METRICS

Measuring Impact

1

Cost Reduction

Reduce cost per new start and achieve ~$1.5M operational savings (reduce cost by 5% in year 1)

2

Scale Efficiency

Support 200k+ and growing student population with 25% self-service rate in year 1

3

Engagement

Improve student engagement and completion rates

4

Staff Ratio

Increase students-to-care-staff ratio significantly

---

# Slide 7

Product Tenets

01

Human Connection First

We help learners get the right information quickly but do not replace the essential human connection in learning.

02

Do the Heavy Lifting

We do for learners what they shouldn’t have to do for themselves.

03

Context-Aware Experiences

We craft meaningful experiences tailored to the learner's context and sentiment so they can choose their next best step.

04

Safeguards & Integrity

We build safeguards and guardrails to ensure support policies are reflected and academic integrity policies are upheld.

05

Security & Privacy

We uphold the highest standards of security and confidentiality in every interaction.

06

Continuous Improvement

We get better with learners through ongoing feedback and measurable outcomes

---

# Slide 8

DESIGN DECISIONS

Scope & Design Decisions

Phase 1 Scope

Start with enrollment - Limited to website data and student handbook public pages

Excluded blog content to maintain focus

Daily embeddings update via scrape-chunk-embed pipeline

Human-in-the-Loop (HITL)

Live human transfer capability required

Full chat transcript visibility in Salesforce

Low confidence scores route to human

User-requested transfers honored immediately

UX Flow

Quick replies for common inquiries on first screen

Bot personality - helpful librarian + friendly guide

Error Handling

Authentication issues

Timeout and latency

Rate limits

Ambiguous questions

Hallucination detection

---

# Slide 9

Technical Architecture

Databricks Model Platform

Custom LLM hosted and trained on WGU content

Genesys Web Messenger

Front-end chat experience and omnichannel platform

Salesforce CRM

Transcript storage and counselor workspace

POCs validated integrations before build phase. Architecture approved despite Genesys limitations due to existing omnichannel investment.

---

# Slide 10

BUILD PHASE

Evaluation Strategy

1

Manual Evaluation Guide

Created rubric for SMEs: pass/fail criteria, criticality ratings (low/medium/high), documentation of glaring issues

2

SME Testing Rounds

Pulled subject matter experts into accuracy and relevance evaluation as soon as model was created

3

Golden Dataset Creation

Used SME responses to build evaluation dataset, evolving into benchmark standard for long-term QA

4

Iterative Refinement

Phase 2 simplified to Pass/Fail with documentation only on failures per rubric category

---

# Slide 11

Results: Dramatic Improvement

81.7%

Accuracy

Up from 15% initially

97.5%

Relevance

Up from 86% initially

Within three months, the team completed critical foundational development. Model trained on all public WGU content with built-in guardrails and source-backed responses. Multi-phase evaluation drove significant improvements through AI engineering, product/UX, and enrollment SME testing.

---

# Slide 12

CHALLENGES

Key Challenges & Solutions

Cross-Functional Alignment

Challenge: 25+ team members across data engineering, ML, product, UX, infrastructure with unclear roles considering this was our first LLM product.

Solution: Built comprehensive roles and responsibilities matrix for development, deployment, and production.

Scope Disagreement

Challenge: Business wanted full website vs. product's FAQ-only recommendation.

Solution: Documented risks (scraping time, evaluation complexity, hallucination) and proceeded with business decision.

Complex HITL Requirements

Challenge: Business insisted on live handoff and Salesforce transcript integration vs. simple contact-us page re-direct.

Solution: Called out technical complexity and timeline risks, proceeded with business priority.

---

# Slide 13

Genesys Platform Limitations

Technical Gaps Identified

No loading indicator for delayed responses (3+ seconds)

No streaming capability for partial responses

No placement for "AI can make mistakes" warning

PII masking applied universally, not per-channel

No in-chat form support unlike Salesforce chat

Recommendations Made

Engage Genesys for roadmap acceleration of critical UX features

Evaluate alternative front-end solutions while keeping Genesys backend

Plan for additional engineering resources (only 2 engineers + 1 architect)

Legal approved proceeding without PII masking for authenticated enrollment experience.

---

# Slide 14

ROADMAP

Enterprise Roadmap

Phase 1: MVP Chatbots

Launch for enrollment and support with human-in-the-loop

Phase 2: Simple Automations

Simple automations (tickets, appointment scheduling) to information retrieval agents

Phase 3: Proactive Nudges

Chatbot-driven engagement

Phase 4: Advanced Use Cases

Tutoring, and motivational support

Phase 5: Agentic Capabilities

Agentic capabilities ranging from simple workflows to complex multi-step workflows

---

# Slide 15

Key Takeaways

Cross-Functional Collaboration

Clear roles and responsibilities critical for 25+ person team success

Rigorous Evaluation

Systematic testing drove accuracy from 15% to 81.7% in three months

Risk Management

Document limitations, propose alternatives, align on trade-offs with stakeholders

Product Tenets

Strong principles guided decisions: human connection first, security, continuous improvement

Building WGU's first LLM chatbot required balancing innovation with pragmatism, technical excellence with business urgency, and AI capabilities with human touch.

---
