---
description: Allianz webhook implementation standard definition
layout: schema
name: WebhookGuideline
properties_list:
- description: Unique identifier for the webhook guideline
  name: guideline_id
  type: string
- description: Name of the guideline
  name: name
  type: string
- description: Version of the guideline
  name: version
  type: string
- description: Supported webhook notification types
  name: notification_types
  type: array
- description: Security requirements for webhook endpoints
  name: security_requirements
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-webhook-guideline-schema.json
slug: tech-standards-webhook-guideline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-webhook-guideline-schema.json\",\n  \"title\": \"WebhookGuideline\",\n  \"description\": \"Allianz webhook implementation standard definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guideline_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the webhook guideline\",\n      \"example\": \"guide-wh-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the guideline\",\n      \"example\": \"Webhook Notification Standard\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the guideline\",\n      \"example\": \"1.3.0\"\n    },\n    \"notification_types\": {\n      \"type\": \"array\",\n      \"description\": \"Supported webhook notification types\"\
  ,\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"security_requirements\": {\n      \"type\": \"array\",\n      \"description\": \"Security requirements for webhook endpoints\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-webhook-guideline-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: WebhookGuideline
---
