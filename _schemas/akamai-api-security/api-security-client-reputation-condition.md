---
description: Collects data needed for condition matches on Client Reputation.
layout: schema
name: client-reputation-condition
properties_list:
- description: The type of condition. In this case, `ClientReputationCondition`.
  name: className
  type: string
- description: Identifies the reputation category. Web scrapers (`WEBSCRP`) crawl sites and collect data like hotel rates, product prices, store locations, and more. DoS attackers (`DOSATCK`) are web clients or botn
  name: name
  type: array
- description: Whether the condition triggers on a match or lack of match.
  name: positiveMatch
  type: boolean
- description: Identifies the IP sharing. Either `NON_SHARED`, `SHARED_ONLY`, `BOTH`.
  name: sharedIpHandling
  type: string
- description: Threshold value that causes the trigger.
  name: value
  type: number
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-client-reputation-condition-schema.json
slug: api-security-client-reputation-condition
source_filename: api-security-client-reputation-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-client-reputation-condition-schema.json\",\n  \"title\": \"client-reputation-condition\",\n  \"description\": \"Collects data needed for condition matches on Client Reputation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"className\": {\n      \"description\": \"The type of condition. In this case, `ClientReputationCondition`.\",\n      \"enum\": [\n        \"ClientReputationCondition\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Identifies the reputation category. Web scrapers (`WEBSCRP`) crawl sites and collect data like hotel rates, product prices, store locations, and more. DoS attackers (`DOSATCK`) are web clients or botnets that use automated tools to launch volumetric Denial of Service (DoS) attacks. Web attackers (`WEBATCK`)\
  \ target websites and web apps with techniques like SQL injection, remote file inclusion, or cross-site scripting. Scanning tools (`SCANTL`) probe web apps for vulnerabilities during an attack's reconnaissance phase.\",\n      \"items\": {\n        \"enum\": [\n          \"WEBSCRP\",\n          \"DOSATCK\",\n          \"WEBATCK\",\n          \"SCANTL\"\n        ],\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"positiveMatch\": {\n      \"description\": \"Whether the condition triggers on a match or lack of match.\",\n      \"type\": \"boolean\"\n    },\n    \"sharedIpHandling\": {\n      \"description\": \"Identifies the IP sharing. Either `NON_SHARED`, `SHARED_ONLY`, `BOTH`.\",\n      \"enum\": [\n        \"NON_SHARED\",\n        \"SHARED_ONLY\",\n        \"BOTH\"\n      ],\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Threshold value that causes the trigger.\",\n\
  \      \"maximum\": 10,\n      \"minimum\": 1,\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"className\",\n    \"name\",\n    \"value\",\n    \"sharedIpHandling\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-client-reputation-condition-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: client-reputation-condition
---
