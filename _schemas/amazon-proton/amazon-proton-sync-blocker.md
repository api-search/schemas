---
description: Detailed data of the sync blocker.
layout: schema
name: SyncBlocker
properties_list:
- description: ''
  name: contexts
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: createdReason
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: resolvedAt
  type: object
- description: ''
  name: resolvedReason
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-sync-blocker-schema.json
slug: amazon-proton-sync-blocker
source_filename: amazon-proton-sync-blocker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-sync-blocker-schema.json\",\n  \"title\": \"SyncBlocker\",\n  \"description\": \"Detailed data of the sync blocker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contexts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncBlockerContexts\"\n        },\n        {\n          \"description\": \"The contexts for the sync blocker.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the sync blocker was created.\"\n        }\n      ]\n    },\n    \"createdReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\
  The reason why the sync blocker was created.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the sync blocker.\"\n        }\n      ]\n    },\n    \"resolvedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the sync blocker was resolved.\"\n        }\n      ]\n    },\n    \"resolvedReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason the sync blocker was resolved.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockerStatus\"\n        },\n        {\n          \"description\": \"The status of the sync blocker.\"\n        }\n      ]\n    },\n    \"type\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockerType\"\n        },\n        {\n          \"description\": \"The type of the sync blocker.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"createdReason\",\n    \"id\",\n    \"status\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-sync-blocker-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: SyncBlocker
---
