---
description: DomainDetail schema from Palo Alto Networks DNS Security API
layout: schema
name: DomainDetail
properties_list:
- description: Fully qualified domain name queried.
  name: domain
  type: string
- description: URL filtering category assigned to the domain (e.g., malware, phishing, command-and-control, business-and-economy).
  name: category
  type: string
- description: Risk level assessment for the domain.
  name: risk_level
  type: string
- description: Numeric risk score from 0.0 (no risk) to 100.0 (critical risk).
  name: risk_score
  type: number
- description: DNS Security category classification used for policy enforcement.
  name: dns_security_category
  type: string
- description: Timestamp when the domain was first observed by DNS Security.
  name: first_seen
  type: string
- description: Timestamp when the domain was most recently observed.
  name: last_seen
  type: string
- description: Domain registrar name.
  name: registrar
  type: string
- description: Date the domain was registered.
  name: registration_date
  type: string
- description: Current IP addresses the domain resolves to.
  name: ip_addresses
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dns-security-api-domain-detail-schema.json
slug: dns-security-api-domain-detail
source_filename: dns-security-api-domain-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DomainDetail\",\n  \"description\": \"DomainDetail schema from Palo Alto Networks DNS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dns-security-api-domain-detail-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified domain name queried.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"URL filtering category assigned to the domain (e.g., malware, phishing, command-and-control, business-and-economy).\"\n    },\n    \"risk_level\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Risk level assessment for the domain.\"\n    },\n    \"risk_score\": {\n      \"type\": \"\
  number\",\n      \"format\": \"float\",\n      \"description\": \"Numeric risk score from 0.0 (no risk) to 100.0 (critical risk).\",\n      \"minimum\": 0.0,\n      \"maximum\": 100.0\n    },\n    \"dns_security_category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"benign\",\n        \"malware\",\n        \"phishing\",\n        \"command-and-control\",\n        \"grayware\",\n        \"dynamic-dns\",\n        \"newly-registered\",\n        \"parked\",\n        \"unknown\"\n      ],\n      \"description\": \"DNS Security category classification used for policy enforcement.\"\n    },\n    \"first_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the domain was first observed by DNS Security.\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the domain was most recently observed.\"\n    },\n    \"registrar\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Domain registrar name.\"\n    },\n    \"registration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the domain was registered.\"\n    },\n    \"ip_addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Current IP addresses the domain resolves to.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dns-security-api-domain-detail-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DomainDetail
---
