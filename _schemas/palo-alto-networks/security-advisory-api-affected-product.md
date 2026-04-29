---
description: AffectedProduct schema from Palo Alto Networks Security Advisory API
layout: schema
name: AffectedProduct
properties_list:
- description: Product name (e.g., PAN-OS, Cortex XDR Agent).
  name: product
  type: string
- description: ''
  name: versions
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/security-advisory-api-affected-product-schema.json
slug: security-advisory-api-affected-product
source_filename: security-advisory-api-affected-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AffectedProduct\",\n  \"description\": \"AffectedProduct schema from Palo Alto Networks Security Advisory API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-affected-product-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Product name (e.g., PAN-OS, Cortex XDR Agent).\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"Affected version or version range.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Affected\",\n              \"Unaffected\",\n              \"Fixed\"\n      \
  \      ],\n            \"description\": \"Vulnerability status for this version.\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-affected-product-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AffectedProduct
---
