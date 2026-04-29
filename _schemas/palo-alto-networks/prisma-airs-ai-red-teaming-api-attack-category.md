---
description: AttackCategory schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: AttackCategory
properties_list:
- description: Unique identifier for the attack category.
  name: category_id
  type: string
- description: Human-readable category name.
  name: name
  type: string
- description: Description of the vulnerability class this category tests.
  name: description
  type: string
- description: Number of built-in attack probes in this category.
  name: attack_count
  type: integer
- description: Severity range of vulnerabilities this category can discover.
  name: severity_range
  type: object
- description: Example attack type names within this category.
  name: examples
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-attack-category-schema.json
slug: prisma-airs-ai-red-teaming-api-attack-category
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttackCategory\",\n  \"description\": \"AttackCategory schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-attack-category-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the attack category.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable category name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the vulnerability class this category tests.\"\n    },\n    \"attack_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of built-in attack probes in this category.\"\n    },\n    \"severity_range\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"Severity range of vulnerabilities this category can discover.\",\n      \"properties\": {\n        \"min\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"informational\",\n            \"low\",\n            \"medium\",\n            \"high\",\n            \"critical\"\n          ]\n        },\n        \"max\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"informational\",\n            \"low\",\n            \"medium\",\n            \"high\",\n            \"critical\"\n          ]\n        }\n      }\n    },\n    \"examples\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Example attack type names within this category.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-attack-category-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AttackCategory
---
