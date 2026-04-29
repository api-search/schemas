---
description: GetTemplateSyncConfigInput schema from Amazon Proton API
layout: schema
name: GetTemplateSyncConfigInput
properties_list:
- description: ''
  name: templateName
  type: object
- description: ''
  name: templateType
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-template-sync-config-input-schema.json
slug: amazon-proton-get-template-sync-config-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-config-input-schema.json\",\n  \"title\": \"GetTemplateSyncConfigInput\",\n  \"description\": \"GetTemplateSyncConfigInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The template name.\"\n        }\n      ]\n    },\n    \"templateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The template type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templateName\",\n    \"templateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-config-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetTemplateSyncConfigInput
---
