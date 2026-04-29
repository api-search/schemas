---
description: Response containing a list of SaaS domains
layout: schema
name: DomainsResponse
properties_list:
- description: ''
  name: domains
  type: array
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-domains-response-schema.json
slug: saas-protection-api-domains-response
source_filename: saas-protection-api-domains-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-domains-response-schema.json\",\n  \"title\": \"DomainsResponse\",\n  \"description\": \"Response containing a list of SaaS domains\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Domain\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-domains-response-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: DomainsResponse
---
