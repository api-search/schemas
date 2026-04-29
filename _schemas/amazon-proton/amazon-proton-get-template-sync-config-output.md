---
description: GetTemplateSyncConfigOutput schema from Amazon Proton API
layout: schema
name: GetTemplateSyncConfigOutput
properties_list:
- description: ''
  name: templateSyncConfig
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-template-sync-config-output-schema.json
slug: amazon-proton-get-template-sync-config-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-config-output-schema.json\",\n  \"title\": \"GetTemplateSyncConfigOutput\",\n  \"description\": \"GetTemplateSyncConfigOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateSyncConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateSyncConfig\"\n        },\n        {\n          \"description\": \"The template sync configuration detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-config-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetTemplateSyncConfigOutput
---
