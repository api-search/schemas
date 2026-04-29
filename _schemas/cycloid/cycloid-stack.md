---
description: A Cycloid Service Catalog Stack template.
layout: schema
name: Stack
properties_list:
- description: Stack reference (organization:stack-canonical).
  name: ref
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: author
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: technologies
  type: array
- description: ''
  name: config_repository_canonical
  type: string
- description: ''
  name: service_catalog_source_canonical
  type: string
provider_name: Cycloid
provider_slug: cycloid
schema_file: json-schema/cycloid-stack-schema.json
slug: cycloid-stack
source_filename: cycloid-stack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/json-schema/cycloid-stack-schema.json\",\n  \"title\": \"Stack\",\n  \"description\": \"A Cycloid Service Catalog Stack template.\",\n  \"type\": \"object\",\n  \"required\": [\"ref\", \"name\"],\n  \"properties\": {\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"Stack reference (organization:stack-canonical).\"\n    },\n    \"name\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"author\": { \"type\": \"string\" },\n    \"version\": { \"type\": \"string\" },\n    \"technologies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"config_repository_canonical\": { \"type\": \"string\" },\n    \"service_catalog_source_canonical\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/json-schema/cycloid-stack-schema.json
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
title: Stack
---
