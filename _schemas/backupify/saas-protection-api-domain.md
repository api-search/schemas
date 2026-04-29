---
description: A SaaS customer domain with backup subscription information
layout: schema
name: Domain
properties_list:
- description: Unique SaaS customer identifier
  name: saasCustomerId
  type: string
- description: External subscription identifier for seat management
  name: externalSubscriptionId
  type: string
- description: The domain name (e.g., company.onmicrosoft.com)
  name: domain
  type: string
- description: Domain backup status
  name: status
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-domain-schema.json
slug: saas-protection-api-domain
source_filename: saas-protection-api-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-domain-schema.json\",\n  \"title\": \"Domain\",\n  \"description\": \"A SaaS customer domain with backup subscription information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"saasCustomerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique SaaS customer identifier\",\n      \"example\": \"cust-001\"\n    },\n    \"externalSubscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"External subscription identifier for seat management\",\n      \"example\": \"sub-abc123\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name (e.g., company.onmicrosoft.com)\",\n      \"example\": \"company.onmicrosoft.com\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Domain backup status\"\
  ,\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-domain-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: Domain
---
