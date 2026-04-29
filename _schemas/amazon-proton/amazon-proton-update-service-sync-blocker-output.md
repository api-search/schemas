---
description: UpdateServiceSyncBlockerOutput schema from Amazon Proton API
layout: schema
name: UpdateServiceSyncBlockerOutput
properties_list:
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
- description: ''
  name: serviceSyncBlocker
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-sync-blocker-output-schema.json
slug: amazon-proton-update-service-sync-blocker-output
source_filename: amazon-proton-update-service-sync-blocker-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-blocker-output-schema.json\",\n  \"title\": \"UpdateServiceSyncBlockerOutput\",\n  \"description\": \"UpdateServiceSyncBlockerOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance that you want to update the service sync blocker for.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that you want to update the service sync blocker for.\"\n        }\n      ]\n    },\n\
  \    \"serviceSyncBlocker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncBlocker\"\n        },\n        {\n          \"description\": \"The detailed data on the service sync blocker that was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\",\n    \"serviceSyncBlocker\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-blocker-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceSyncBlockerOutput
---
