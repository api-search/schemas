---
description: UpdateServiceSyncBlockerInput schema from Amazon Proton API
layout: schema
name: UpdateServiceSyncBlockerInput
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: resolvedReason
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-sync-blocker-input-schema.json
slug: amazon-proton-update-service-sync-blocker-input
source_filename: amazon-proton-update-service-sync-blocker-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-blocker-input-schema.json\",\n  \"title\": \"UpdateServiceSyncBlockerInput\",\n  \"description\": \"UpdateServiceSyncBlockerInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the service sync blocker.\"\n        }\n      ]\n    },\n    \"resolvedReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason the service sync blocker was resolved.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"resolvedReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-blocker-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceSyncBlockerInput
---
