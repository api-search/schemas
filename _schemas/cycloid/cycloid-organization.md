---
description: A Cycloid organization tenant.
layout: schema
name: Organization
properties_list:
- description: URL-safe slug used in API paths.
  name: canonical
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: owner
  type: object
provider_name: Cycloid
provider_slug: cycloid
schema_file: json-schema/cycloid-organization-schema.json
slug: cycloid-organization
source_filename: cycloid-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/json-schema/cycloid-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"A Cycloid organization tenant.\",\n  \"type\": \"object\",\n  \"required\": [\"canonical\", \"name\"],\n  \"properties\": {\n    \"canonical\": {\n      \"type\": \"string\",\n      \"description\": \"URL-safe slug used in API paths.\"\n    },\n    \"name\": { \"type\": \"string\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updated_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"username\": { \"type\": \"string\" },\n        \"email\": { \"type\": \"string\", \"format\": \"email\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/json-schema/cycloid-organization-schema.json
tags:
- Asset Inventory
- CI/CD
- Cloud Cost Management
- Cloud Management
- Developer Experience
- DevOps
- FinOps
- GitOps
- GreenOps
- Infrastructure as Code
- Internal Developer Platform
- Internal Developer Portal
- Multi-Cloud
- Platform Engineering
- RBAC
- Self-Service
- Service Catalog
- StackForms
- Terraform
title: Organization
---
