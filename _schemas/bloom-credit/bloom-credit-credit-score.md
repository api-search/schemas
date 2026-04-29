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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bloom-credit/main/json-schema/bloom-credit-credit-score-schema.json\",\n  \"title\": \"CreditScore\",\n  \"description\": \"A credit score from a specific bureau and scoring model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bureau\": {\n      \"type\": \"string\",\n      \"description\": \"Credit bureau providing the score.\",\n      \"enum\": [\"equifax\", \"experian\", \"transunion\"],\n      \"example\": \"equifax\"\n    },\n    \"score_type\": {\n      \"type\": \"string\",\n      \"description\": \"Scoring model used (e.g., FICO8, VANTAGE3).\",\n      \"example\": \"FICO8\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"Numerical credit score value.\",\n      \"minimum\": 300,\n      \"maximum\": 850,\n      \"example\": 720\n    },\n    \"score_range_min\": {\n      \"type\": \"integer\",\n \
  \     \"description\": \"Minimum score in the scoring model range.\",\n      \"example\": 300\n    },\n    \"score_range_max\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum score in the scoring model range.\",\n      \"example\": 850\n    },\n    \"factors\": {\n      \"type\": \"array\",\n      \"description\": \"Score factors and reasons.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": { \"type\": \"string\", \"example\": \"PAYMENT_HISTORY\" },\n          \"description\": { \"type\": \"string\", \"example\": \"Payments made on time\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/json-schema/bloom-credit-credit-score-schema.json
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: CreditScore
---
