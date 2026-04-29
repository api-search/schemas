---
description: UpdateServiceSyncConfigOutput schema from Amazon Proton API
layout: schema
name: UpdateServiceSyncConfigOutput
properties_list:
- description: ''
  name: serviceSyncConfig
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-sync-config-output-schema.json
slug: amazon-proton-update-service-sync-config-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-config-output-schema.json\",\n  \"title\": \"UpdateServiceSyncConfigOutput\",\n  \"description\": \"UpdateServiceSyncConfigOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceSyncConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceSyncConfig\"\n        },\n        {\n          \"description\": \"The detailed data of the Proton Ops file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-config-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceSyncConfigOutput
---
