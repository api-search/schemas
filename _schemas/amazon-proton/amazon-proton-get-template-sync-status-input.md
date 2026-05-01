---
description: GetTemplateSyncStatusInput schema from Amazon Proton API
layout: schema
name: GetTemplateSyncStatusInput
properties_list:
- description: ''
  name: templateName
  type: object
- description: ''
  name: templateType
  type: object
- description: ''
  name: templateVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-template-sync-status-input-schema.json
slug: amazon-proton-get-template-sync-status-input
source_filename: amazon-proton-get-template-sync-status-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-status-input-schema.json\",\n  \"title\": \"GetTemplateSyncStatusInput\",\n  \"description\": \"GetTemplateSyncStatusInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The template name.\"\n        }\n      ]\n    },\n    \"templateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The template type.\"\n        }\n      ]\n    },\n    \"templateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n\
  \          \"description\": \"The template major version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templateName\",\n    \"templateType\",\n    \"templateVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-template-sync-status-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetTemplateSyncStatusInput
---
