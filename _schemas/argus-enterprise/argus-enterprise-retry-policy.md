---
description: RetryPolicy schema from ARGUS Enterprise API
layout: schema
name: RetryPolicy
properties_list:
- description: Maximum number of delivery retry attempts
  name: maxRetries
  type: integer
- description: Initial interval between retries in seconds
  name: retryIntervalSeconds
  type: integer
- description: Exponential backoff multiplier
  name: backoffMultiplier
  type: number
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-retry-policy-schema.json
slug: argus-enterprise-retry-policy
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: RetryPolicy
---
