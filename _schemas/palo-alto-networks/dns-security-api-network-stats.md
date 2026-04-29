---
description: NetworkStats schema from Palo Alto Networks DNS Security API
layout: schema
name: NetworkStats
properties_list:
- description: Customer ID for which statistics are returned.
  name: customerid
  type: string
- description: ''
  name: period
  type: object
- description: Total DNS queries processed during the period.
  name: total_queries
  type: integer
- description: DNS queries blocked by DNS Security policy.
  name: blocked_queries
  type: integer
- description: DNS queries allowed by DNS Security policy.
  name: allowed_queries
  type: integer
- description: DNS queries redirected to sinkhole.
  name: sinkholed_queries
  type: integer
- description: Most frequently queried domains during the period.
  name: top_queried_domains
  type: array
- description: Query counts grouped by DNS Security category.
  name: category_breakdown
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dns-security-api-network-stats-schema.json
slug: dns-security-api-network-stats
source_filename: dns-security-api-network-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkStats\",\n  \"description\": \"NetworkStats schema from Palo Alto Networks DNS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dns-security-api-network-stats-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerid\": {\n      \"type\": \"string\",\n      \"description\": \"Customer ID for which statistics are returned.\"\n    },\n    \"period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"description\": \"Start of the statistics period.\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"description\": \"End of the statistics period.\"\n        }\n      }\n    },\n    \"total_queries\": {\n      \"type\": \"integer\",\n      \"description\": \"Total DNS queries processed during the\
  \ period.\"\n    },\n    \"blocked_queries\": {\n      \"type\": \"integer\",\n      \"description\": \"DNS queries blocked by DNS Security policy.\"\n    },\n    \"allowed_queries\": {\n      \"type\": \"integer\",\n      \"description\": \"DNS queries allowed by DNS Security policy.\"\n    },\n    \"sinkholed_queries\": {\n      \"type\": \"integer\",\n      \"description\": \"DNS queries redirected to sinkhole.\"\n    },\n    \"top_queried_domains\": {\n      \"type\": \"array\",\n      \"description\": \"Most frequently queried domains during the period.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"domain\": {\n            \"type\": \"string\"\n          },\n          \"query_count\": {\n            \"type\": \"integer\"\n          },\n          \"dns_security_category\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"category_breakdown\": {\n      \"type\": \"array\",\n      \"description\": \"Query\
  \ counts grouped by DNS Security category.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category\": {\n            \"type\": \"string\"\n          },\n          \"count\": {\n            \"type\": \"integer\"\n          },\n          \"percentage\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dns-security-api-network-stats-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NetworkStats
---
