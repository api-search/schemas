---
description: Product schema from Palo Alto Networks Security Advisory API
layout: schema
name: Product
properties_list:
- description: Product name as referenced in advisories.
  name: name
  type: string
- description: Number of published advisories referencing this product.
  name: advisory_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/security-advisory-api-product-schema.json
slug: security-advisory-api-product
source_filename: security-advisory-api-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Product\",\n  \"description\": \"Product schema from Palo Alto Networks Security Advisory API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-product-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name as referenced in advisories.\"\n    },\n    \"advisory_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of published advisories referencing this product.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-product-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Product
---
