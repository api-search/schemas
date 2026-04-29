---
description: A DNS record object from the Cloudflare API, representing a single DNS record entry within a zone. Supports all standard record types including A, AAAA, CNAME, MX, TXT, SRV, and more.
layout: schema
name: Cloudflare DNS Record
properties_list:
- description: The unique identifier of the DNS record.
  name: id
  type: string
- description: The zone identifier this record belongs to.
  name: zone_id
  type: string
- description: The domain name of the zone.
  name: zone_name
  type: string
- description: The type of DNS record.
  name: type
  type: string
- description: The DNS record name (fully qualified domain name).
  name: name
  type: string
- description: The value of the DNS record. Content format depends on the record type.
  name: content
  type: string
- description: Time to live in seconds. A value of 1 indicates automatic TTL managed by Cloudflare.
  name: ttl
  type: integer
- description: Record priority, required for MX, SRV, and URI record types.
  name: priority
  type: integer
- description: Whether the record is receiving the performance and security benefits of Cloudflare's proxy.
  name: proxied
  type: boolean
- description: Whether the record can be proxied through Cloudflare.
  name: proxiable
  type: boolean
- description: Whether the record is locked and cannot be modified.
  name: locked
  type: boolean
- description: A comment about the DNS record for documentation purposes.
  name: comment
  type: string
- description: Custom tags for categorizing and filtering DNS records.
  name: tags
  type: array
- description: Structured data for record types that require additional fields (SRV, CAA, SSHFP, etc.).
  name: data
  type: object
- description: Extra Cloudflare-specific metadata about the record.
  name: meta
  type: object
- description: When the record was created.
  name: created_on
  type: string
- description: When the record was last modified.
  name: modified_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-dns-record-schema.json
slug: cloudflare-dns-record
source_filename: cloudflare-dns-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-dns-record-schema.json\",\n  \"title\": \"Cloudflare DNS Record\",\n  \"description\": \"A DNS record object from the Cloudflare API, representing a single DNS record entry within a zone. Supports all standard record types including A, AAAA, CNAME, MX, TXT, SRV, and more.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"name\", \"content\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the DNS record.\"\n    },\n    \"zone_id\": {\n      \"type\": \"string\",\n      \"description\": \"The zone identifier this record belongs to.\"\n    },\n    \"zone_name\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name of the zone.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The type of DNS record.\",\n      \"enum\": [\n        \"A\", \"AAAA\", \"CAA\", \"CERT\", \"CNAME\", \"DNSKEY\", \"DS\", \"HTTPS\",\n        \"LOC\", \"MX\", \"NAPTR\", \"NS\", \"PTR\", \"SMIMEA\", \"SRV\", \"SSHFP\",\n        \"SVCB\", \"TLSA\", \"TXT\", \"URI\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS record name (fully qualified domain name).\",\n      \"maxLength\": 255\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the DNS record. Content format depends on the record type.\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to live in seconds. A value of 1 indicates automatic TTL managed by Cloudflare.\",\n      \"minimum\": 1,\n      \"maximum\": 86400\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Record priority, required for MX, SRV, and URI record types.\",\n      \"minimum\": 0,\n      \"maximum\"\
  : 65535\n    },\n    \"proxied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record is receiving the performance and security benefits of Cloudflare's proxy.\"\n    },\n    \"proxiable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record can be proxied through Cloudflare.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record is locked and cannot be modified.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment about the DNS record for documentation purposes.\",\n      \"maxLength\": 100\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 36\n      },\n      \"description\": \"Custom tags for categorizing and filtering DNS records.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Structured data for record types that require additional\
  \ fields (SRV, CAA, SSHFP, etc.).\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Extra Cloudflare-specific metadata about the record.\",\n      \"properties\": {\n        \"auto_added\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the record was auto-added by Cloudflare.\"\n        },\n        \"managed_by_apps\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the record is managed by a Cloudflare app.\"\n        },\n        \"managed_by_argo_tunnel\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the record is managed by a Cloudflare Tunnel.\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The source of the DNS record.\"\n        }\n      }\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the record was created.\"\n    },\n    \"modified_on\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the record was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-dns-record-schema.json
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
title: Cloudflare DNS Record
---
