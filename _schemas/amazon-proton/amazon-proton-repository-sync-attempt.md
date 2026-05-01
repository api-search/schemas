---
description: Detail data for a repository sync attempt activated by a push to a repository.
layout: schema
name: RepositorySyncAttempt
properties_list:
- description: ''
  name: events
  type: object
- description: ''
  name: startedAt
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-repository-sync-attempt-schema.json
slug: amazon-proton-repository-sync-attempt
source_filename: amazon-proton-repository-sync-attempt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-attempt-schema.json\",\n  \"title\": \"RepositorySyncAttempt\",\n  \"description\": \"Detail data for a repository sync attempt activated by a push to a repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySyncEvents\"\n        },\n        {\n          \"description\": \"Detail data for sync attempt events.\"\n        }\n      ]\n    },\n    \"startedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the sync attempt started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySyncStatus\"\
  \n        },\n        {\n          \"description\": \"The sync attempt status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"events\",\n    \"startedAt\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-attempt-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: RepositorySyncAttempt
---
