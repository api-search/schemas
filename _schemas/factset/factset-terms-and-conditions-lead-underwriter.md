---
description: Lead Underwriter for a Fixed Income security.
layout: schema
name: leadUnderwriter
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: FactSet Entity Id for Lead Underwriter.
  name: factsetLeadUwritrEntityId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-lead-underwriter-schema.json
slug: factset-terms-and-conditions-lead-underwriter
source_filename: factset-terms-and-conditions-lead-underwriter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"leadUnderwriter\",\n  \"type\": \"object\",\n  \"description\": \"Lead Underwriter for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"factsetLeadUwritrEntityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Id for Lead Underwriter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-lead-underwriter-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: leadUnderwriter
---
