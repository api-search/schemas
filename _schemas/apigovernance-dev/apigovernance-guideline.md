---
description: An API governance guideline or best practice.
layout: schema
name: Guideline
properties_list:
- description: Unique identifier for the guideline.
  name: id
  type: string
- description: Governance category (e.g., Security, Design, Documentation).
  name: category
  type: string
- description: Short title of the guideline.
  name: title
  type: string
- description: Detailed description of the guideline.
  name: description
  type: string
- description: Severity level of violation.
  name: severity
  type: string
- description: Tags categorizing the guideline.
  name: tags
  type: array
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-guideline-schema.json
slug: apigovernance-guideline
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Guideline
---
