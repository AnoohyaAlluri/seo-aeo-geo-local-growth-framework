# Schema Examples

## Purpose

This document explains public-safe schema and structured-data examples for the SEO, AEO, and GEO website growth framework.

Schema helps search engines and AI systems understand page type, business context, service areas, FAQs, articles, and content relationships.

---

## Why Schema Matters

Schema and structured data can help clarify:

* What type of page is being shown
* What service is being described
* What location or service area is relevant
* Which FAQs belong to the page
* Whether the page is a guide, service page, city page, or article
* How business entities, services, and locations connect

Schema does not replace strong content. It supports clearer interpretation of the content already present on the page.

---

## Recommended Schema by Page Type

| Page Type | Recommended Schema | Purpose |
| --------- | ------------------ | ------- |
| Homepage | LocalBusiness | Identifies the business and general service area |
| Service Page | Service | Defines the service offering |
| City Page | LocalBusiness or Service | Connects service offering to a local area |
| Guide Page | Article | Supports educational or long-form informational content |
| FAQ Page | FAQPage | Structures question-and-answer content |
| Blog Index | CollectionPage | Organizes a collection of articles or resources |

---

## LocalBusiness Schema Example

Use this type for a homepage or major local service page.

```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Example Property Management Company",
  "description": "A local property management company providing leasing, maintenance coordination, tenant communication, and owner support services.",
  "areaServed": [
    "Los Angeles",
    "Santa Monica",
    "Beverly Hills",
    "West Hollywood",
    "Brentwood",
    "Malibu"
  ],
  "serviceType": "Property Management",
  "url": "https://www.example.com"
}
```

---

## Service Schema Example

Use this type for a core service page.

```json
{
  "@context": "https://schema.org",
  "@type": "Service",
  "name": "Property Management Services",
  "description": "Property management services for rental owners, including leasing support, tenant communication, maintenance coordination, reporting, and compliance coordination.",
  "serviceType": "Property Management",
  "areaServed": {
    "@type": "Place",
    "name": "Los Angeles"
  },
  "provider": {
    "@type": "LocalBusiness",
    "name": "Example Property Management Company"
  }
}
```

---

## City Page Schema Example

Use this type for a city-specific service page.

```json
{
  "@context": "https://schema.org",
  "@type": "Service",
  "name": "Santa Monica Property Management Services",
  "description": "Property management services for rental owners in Santa Monica, including leasing, maintenance coordination, tenant communication, and owner reporting.",
  "serviceType": "Property Management",
  "areaServed": {
    "@type": "City",
    "name": "Santa Monica"
  },
  "provider": {
    "@type": "LocalBusiness",
    "name": "Example Property Management Company"
  }
}
```

---

## FAQPage Schema Example

Use this type when a page includes a clear FAQ section.

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What does property management include?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Property management may include leasing, tenant communication, maintenance coordination, rent collection support, reporting, and compliance-related coordination."
      }
    },
    {
      "@type": "Question",
      "name": "How do I choose a property manager?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Owners should evaluate local experience, communication standards, service coverage, reporting quality, maintenance coordination, and contract structure."
      }
    }
  ]
}
```

---

## Article Schema Example

Use this type for guide pages or educational blog posts.

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "How to Choose a Property Manager",
  "description": "A guide explaining how rental owners can evaluate property management companies based on service scope, communication standards, reporting quality, maintenance coordination, and contract structure.",
  "author": {
    "@type": "Person",
    "name": "Portfolio Author"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Example Organization"
  }
}
```

---

## CollectionPage Schema Example

Use this type for a blog index, resource hub, or educational content library.

```json
{
  "@context": "https://schema.org",
  "@type": "CollectionPage",
  "name": "Property Management Resource Hub",
  "description": "A collection of educational resources for rental owners covering property management, leasing, maintenance coordination, pricing, and owner decision-making."
}
```

---

## Schema Planning Workflow

```text
Identify page type
      ↓
Select recommended schema type
      ↓
Map the page topic
      ↓
Map the service or location entity
      ↓
Write public-safe structured data
      ↓
Validate syntax
      ↓
Document status in content inventory
```

---

## Schema Quality Rules

Schema examples should be:

* Accurate to the visible page content
* Aligned with the page type
* Written in valid JSON-LD format
* Public-safe
* Free of private company information
* Free of internal URLs or account IDs
* Consistent with the page’s actual topic
* Documented in the content tracker

---

## Common Schema Mistakes to Avoid

Avoid:

* Adding schema that does not match the visible page content
* Using fake reviews, fake ratings, or unsupported claims
* Including private company data
* Including internal URLs
* Reusing the same schema across unrelated page types
* Marking content as FAQPage if the page does not actually show FAQs
* Adding unsupported business claims or unverifiable metrics

---

## AEO and GEO Benefits

Schema supports AEO and GEO by helping clarify:

* Page purpose
* Entity relationships
* Service categories
* Location relevance
* FAQ structure
* Article or guide context
* Internal content hierarchy

Structured data should work together with clear headings, answer-first content, FAQs, internal links, and strong page architecture.

---

## Public-Safe Note

These schema examples are synthetic and generalized for portfolio demonstration. They do not include private company details, real URLs, account IDs, internal analytics data, client information, tenant information, owner information, or confidential business data.
