# Project Architecture

## Purpose

This document provides the visual architecture for the SEO, AEO, and GEO Website Growth Framework.

The project shows how search-intent research, city-page planning, answer-first content, FAQ structure, schema planning, internal linking, and conversion paths can be organized into a repeatable website growth system.

---

## 1. End-to-End SEO/AEO/GEO Framework

```mermaid
flowchart TD
    A[Search Intent Research] --> B[Topic and City Clustering]
    B --> C[Page Type Mapping]
    C --> D[Answer-First Content Structure]
    D --> E[FAQ Planning]
    E --> F[Schema Recommendation]
    F --> G[Internal Linking Map]
    G --> H[CTA and Conversion Path]
    H --> I[Content Inventory Tracker]
    I --> J[Optimization Summary Outputs]
```

---

## 2. Content Operations Architecture

```mermaid
flowchart LR
    A[Mock Keyword Intent Map] --> B[Content Inventory]
    B --> C[City Page Status Tracker]
    C --> D[Content Gap Summary]
    D --> E[Page Optimization Summary]
    E --> F[Prioritized SEO/AEO/GEO Actions]
```

---

## 3. Page Type Strategy

```mermaid
flowchart TD
    A[Website Growth Framework] --> B[Service Pages]
    A --> C[City Pages]
    A --> D[Guide Pages]
    A --> E[FAQ Pages]
    A --> F[Blog Index Pages]

    B --> B1[Explain Core Services]
    C --> C1[Capture Local Service Intent]
    D --> D1[Answer High-Intent Research Questions]
    E --> E1[Support Answer Engine Visibility]
    F --> F1[Organize Educational Content]
```

---

## 4. City Page Architecture

```mermaid
flowchart TD
    A[City Page] --> B[Hero Section]
    B --> C[Answer-First Section]
    C --> D[Local Service Overview]
    D --> E[Service Process]
    E --> F[Local Trust Section]
    F --> G[FAQ Section]
    G --> H[Internal Links]
    H --> I[Conversion CTA]
```

---

## 5. Answer-First Content Model

```mermaid
flowchart TD
    A[User Question] --> B[Direct Answer]
    B --> C[Supporting Explanation]
    C --> D[Service or Location Context]
    D --> E[FAQ Block]
    E --> F[Related Internal Links]
    F --> G[CTA]
```

---

## 6. FAQ and Schema Workflow

```mermaid
flowchart TD
    A[Identify User Questions] --> B[Group by Intent]
    B --> C[Write Direct FAQ Answers]
    C --> D[Place FAQs on Relevant Page]
    D --> E[Select FAQPage Schema When Appropriate]
    E --> F[Validate Structured Data]
    F --> G[Track Schema Status in Inventory]
```

---

## 7. Internal Linking Architecture

```mermaid
flowchart TD
    A[Homepage] --> B[Core Service Pages]
    B --> C[Priority City Pages]
    C --> D[Guide Pages]
    D --> E[FAQ Hub]
    E --> F[Contact or Consultation Page]

    D --> B
    E --> B
    C --> B
```

---

## 8. AI Visibility Architecture

```mermaid
flowchart TD
    A[Entity-Focused Content] --> B[Service Entity]
    A --> C[Location Entity]
    A --> D[Audience Entity]
    A --> E[Problem Entity]
    A --> F[Conversion Action]

    B --> G[AI-Readable Page Structure]
    C --> G
    D --> G
    E --> G
    F --> G

    G --> H[Answer-First Content]
    H --> I[FAQ Block]
    I --> J[Schema Planning]
    J --> K[Internal Links]
    K --> L[Conversion CTA]
```

---

## 9. Repository Architecture

```mermaid
flowchart TD
    A[seo-aeo-geo-local-growth-framework] --> B[datasets/mock]
    A --> C[docs]
    A --> D[outputs]
    A --> E[images]
    A --> F[README.md]

    B --> B1[content_inventory_mock.csv]
    B --> B2[keyword_intent_map_mock.csv]
    B --> B3[city_page_status_mock.csv]

    C --> C1[requirements.md]
    C --> C2[content_architecture.md]
    C --> C3[city_page_template.md]
    C --> C4[faq_structure.md]
    C --> C5[internal_linking_map.md]
    C --> C6[schema_examples.md]
    C --> C7[ai_visibility_framework.md]
    C --> C8[project_architecture.md]
    C --> C9[case_study.md]

    D --> D1[mock_content_gap_summary.csv]
    D --> D2[mock_page_optimization_summary.csv]
```

---

## 10. Optimization Priority Workflow

```mermaid
flowchart TD
    A[Review Content Inventory] --> B{Is Page Optimized?}
    B -->|Yes| C[Monitor and Refresh Quarterly]
    B -->|No| D[Identify Primary Gap]
    D --> E{Gap Type}
    E -->|FAQ Gap| F[Add FAQ Section]
    E -->|Schema Gap| G[Document Schema Recommendation]
    E -->|Internal Linking Gap| H[Add Relevant Internal Links]
    E -->|CTA Gap| I[Align Page with Conversion Action]
    E -->|Answer Gap| J[Add Answer-First Section]
    F --> K[Update Page Optimization Summary]
    G --> K
    H --> K
    I --> K
    J --> K
```

---

## 11. Strategic Layers

| Layer | Purpose | Example File |
| ---- | ------- | ------------ |
| Research Layer | Organizes keywords, intent, and page mapping | `datasets/mock/keyword_intent_map_mock.csv` |
| Content Inventory Layer | Tracks page type, status, priority, and AI visibility goals | `datasets/mock/content_inventory_mock.csv` |
| City Page Layer | Tracks city-page status, FAQ coverage, schema status, and CTA alignment | `datasets/mock/city_page_status_mock.csv` |
| Documentation Layer | Explains templates, linking logic, schema, and AI visibility | `docs/` |
| Output Layer | Summarizes content gaps and optimization priorities | `outputs/` |
| Portfolio Layer | Presents the project for recruiters and hiring managers | `README.md` |

---

## 12. Business Logic Summary

This project uses a structured workflow:

1. Identify user search intent.
2. Map intent to page type.
3. Organize pages by city, service, and funnel stage.
4. Add answer-first sections.
5. Add FAQ blocks.
6. Document schema recommendations.
7. Add internal links.
8. Align each page with a conversion CTA.
9. Track optimization status.
10. Summarize gaps and priorities.

---

## Public-Safe Note

These diagrams are public-safe visual reconstructions. They do not include private company strategy documents, real analytics exports, internal URLs, account IDs, client information, tenant information, owner information, or confidential business data.
