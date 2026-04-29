---
description: ''
layout: schema
name: DnsRecord
properties_list:
- description: The unique identifier of the DNS record.
  name: id
  type: string
- description: The zone identifier.
  name: zone_id
  type: string
- description: The zone name.
  name: zone_name
  type: string
- description: The DNS record name.
  name: name
  type: string
- description: The DNS record content.
  name: content
  type: string
- description: Time to live in seconds.
  name: ttl
  type: integer
- description: Whether the record is proxied through Cloudflare.
  name: proxied
  type: boolean
- description: Whether the record can be proxied.
  name: proxiable
  type: boolean
- description: Whether the record is locked.
  name: locked
  type: boolean
- description: A comment about the DNS record.
  name: comment
  type: string
- description: Custom tags for the DNS record.
  name: tags
  type: array
- description: When the record was created.
  name: created_on
  type: string
- description: When the record was last modified.
  name: modified_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-dns-dns-record-schema.json
slug: cloudflare-dns-dns-record
source_filename: cloudflare-dns-dns-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DnsRecord\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the DNS record.\"\n    },\n    \"zone_id\": {\n      \"type\": \"string\",\n      \"description\": \"The zone identifier.\"\n    },\n    \"zone_name\": {\n      \"type\": \"string\",\n      \"description\": \"The zone name.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS record name.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS record content.\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to live in seconds.\"\n    },\n    \"proxied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record is proxied through Cloudflare.\"\n    },\n    \"proxiable\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether the record can be proxied.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record is locked.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment about the DNS record.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom tags for the DNS record.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the record was created.\"\n    },\n    \"modified_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the record was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-dns-dns-record-schema.json
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
title: DnsRecord
---
