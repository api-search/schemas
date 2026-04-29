---
description: ''
layout: schema
name: DnsRecordInput
properties_list:
- description: The DNS record name, e.g. example.com.
  name: name
  type: string
- description: The DNS record content value.
  name: content
  type: string
- description: Time to live in seconds. A value of 1 indicates automatic TTL.
  name: ttl
  type: integer
- description: Required for MX, SRV, and URI records. Record priority.
  name: priority
  type: integer
- description: Whether the record is receiving Cloudflare proxy services.
  name: proxied
  type: boolean
- description: A comment about the DNS record.
  name: comment
  type: string
- description: Custom tags for the DNS record.
  name: tags
  type: array
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-dns-dns-record-input-schema.json
slug: cloudflare-dns-dns-record-input
source_filename: cloudflare-dns-dns-record-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DnsRecordInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS record name, e.g. example.com.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS record content value.\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to live in seconds. A value of 1 indicates automatic TTL.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Required for MX, SRV, and URI records. Record priority.\"\n    },\n    \"proxied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record is receiving Cloudflare proxy services.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment about the DNS record.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Custom tags for the DNS record.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-dns-dns-record-input-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: DnsRecordInput
---
