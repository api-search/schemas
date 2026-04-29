---
description: GetTemplateSyncStatusOutput schema from Amazon Proton API
layout: schema
name: GetTemplateSyncStatusOutput
properties_list:
- description: ''
  name: desiredState
  type: object
- description: ''
  name: latestSuccessfulSync
  type: object
- description: ''
  name: latestSync
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-template-sync-status-output-schema.json
slug: amazon-proton-get-template-sync-status-output
source_filename: amazon-proton-get-template-sync-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-status-output-schema.json\",\n  \"title\": \"GetTemplateSyncStatusOutput\",\n  \"description\": \"GetTemplateSyncStatusOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"The template sync desired state that's returned by Proton.\"\n        }\n      ]\n    },\n    \"latestSuccessfulSync\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceSyncAttempt\"\n        },\n        {\n          \"description\": \"The details of the last successful sync that's returned by Proton.\"\n        }\n      ]\n    },\n    \"latestSync\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ResourceSyncAttempt\"\n        },\n        {\n          \"description\": \"The details of the last sync that's returned by Proton.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-status-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetTemplateSyncStatusOutput
---
