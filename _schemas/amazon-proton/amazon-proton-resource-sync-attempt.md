---
description: Detail data for a resource sync attempt activated by a push to a repository.
layout: schema
name: ResourceSyncAttempt
properties_list:
- description: ''
  name: events
  type: object
- description: ''
  name: initialRevision
  type: object
- description: ''
  name: startedAt
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: target
  type: object
- description: ''
  name: targetRevision
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-resource-sync-attempt-schema.json
slug: amazon-proton-resource-sync-attempt
source_filename: amazon-proton-resource-sync-attempt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-sync-attempt-schema.json\",\n  \"title\": \"ResourceSyncAttempt\",\n  \"description\": \"Detail data for a resource sync attempt activated by a push to a repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceSyncEvents\"\n        },\n        {\n          \"description\": \"An array of events with detail data.\"\n        }\n      ]\n    },\n    \"initialRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"Detail data for the initial repository commit, path and push.\"\n        }\n      ]\n    },\n    \"startedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time when the sync attempt started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceSyncStatus\"\n        },\n        {\n          \"description\": \"The status of the sync attempt.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The resource that is synced to.\"\n        }\n      ]\n    },\n    \"targetRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"Detail data for the target revision.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"events\",\n    \"initialRevision\",\n    \"startedAt\",\n    \"status\",\n    \"target\",\n    \"targetRevision\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-sync-attempt-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ResourceSyncAttempt
---
