---
description: A Reserved Domain is a custom hostname reserved for use with HTTP, HTTPS, or TLS tunnels and edges.
layout: schema
name: ngrok Reserved Domain
properties_list:
- description: Unique identifier for the reserved domain.
  name: id
  type: string
- description: URI of the reserved domain API resource.
  name: uri
  type: string
- description: Timestamp when the reserved domain was created.
  name: created_at
  type: string
- description: Human-readable description.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: The hostname of the reserved domain.
  name: domain
  type: string
- description: The ngrok region where the domain is reserved.
  name: region
  type: string
- description: The DNS CNAME target for custom domains.
  name: cname_target
  type: string
- description: Reference to the TLS certificate for the domain.
  name: certificate
  type: object
- description: The certificate management policy for automated TLS certificates.
  name: certificate_management_policy
  type: object
- description: The status of the certificate management process.
  name: certificate_management_status
  type: object
- description: The CNAME target for ACME certificate validation challenges.
  name: acme_challenge_cname_target
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/reserved-domain.json
slug: reserved-domain
source_filename: reserved-domain.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/reserved-domain.json\",\n  \"title\": \"ngrok Reserved Domain\",\n  \"description\": \"A Reserved Domain is a custom hostname reserved for use with HTTP, HTTPS, or TLS tunnels and edges.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the reserved domain.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the reserved domain API resource.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the reserved domain was created.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Arbitrary user-defined metadata.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname of the reserved domain.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The ngrok region where the domain is reserved.\"\n    },\n    \"cname_target\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS CNAME target for custom domains.\"\n    },\n    \"certificate\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the TLS certificate for the domain.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"certificate_management_policy\": {\n      \"type\": \"object\",\n      \"description\": \"The certificate management policy for automated TLS certificates.\"\n    },\n    \"certificate_management_status\": {\n      \"type\": \"object\",\n      \"description\": \"The status\
  \ of the certificate management process.\"\n    },\n    \"acme_challenge_cname_target\": {\n      \"type\": \"string\",\n      \"description\": \"The CNAME target for ACME certificate validation challenges.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/reserved-domain.json
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
title: ngrok Reserved Domain
---
