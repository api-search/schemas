---
description: An API governance policy composed of multiple guidelines.
layout: schema
name: Policy
properties_list:
- description: Policy identifier.
  name: id
  type: string
- description: Policy name.
  name: name
  type: string
- description: Policy description.
  name: description
  type: string
- description: List of guideline IDs included in this policy.
  name: guidelines
  type: array
- description: How this policy is enforced.
  name: enforcement
  type: string
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-policy-schema.json
slug: apigovernance-policy
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Policy
---
