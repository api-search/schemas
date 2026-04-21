---
description: A credit score from a specific bureau and scoring model.
layout: schema
name: CreditScore
properties_list:
- description: Credit bureau providing the score.
  name: bureau
  type: string
- description: Scoring model used (e.g., FICO8, VANTAGE3).
  name: score_type
  type: string
- description: Numerical credit score value.
  name: score
  type: integer
- description: Minimum score in the scoring model range.
  name: score_range_min
  type: integer
- description: Maximum score in the scoring model range.
  name: score_range_max
  type: integer
- description: Score factors and reasons.
  name: factors
  type: array
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-credit-score-schema.json
slug: bloom-credit-credit-score
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: CreditScore
---
