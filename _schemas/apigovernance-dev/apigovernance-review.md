---
description: An automated API governance review result.
layout: schema
name: Review
properties_list:
- description: Review identifier.
  name: id
  type: string
- description: URL of the reviewed API specification.
  name: apiSpecUrl
  type: string
- description: Overall governance score.
  name: score
  type: number
- description: Number of guideline violations found.
  name: violations
  type: integer
- description: When the review was created.
  name: createdAt
  type: string
- description: Review status.
  name: status
  type: string
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-review-schema.json
slug: apigovernance-review
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Review
---
