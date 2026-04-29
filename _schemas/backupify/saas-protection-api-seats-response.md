---
description: Response containing a list of seats for a customer
layout: schema
name: SeatsResponse
properties_list:
- description: ''
  name: seats
  type: array
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-seats-response-schema.json
slug: saas-protection-api-seats-response
source_filename: saas-protection-api-seats-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seats-response-schema.json\",\n  \"title\": \"SeatsResponse\",\n  \"description\": \"Response containing a list of seats for a customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"seats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Seat\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seats-response-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: SeatsResponse
---
