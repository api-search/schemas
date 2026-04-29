---
description: UpdateEnvironmentTemplateInput schema from Amazon Proton API
layout: schema
name: UpdateEnvironmentTemplateInput
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-environment-template-input-schema.json
slug: amazon-proton-update-environment-template-input
source_filename: amazon-proton-update-environment-template-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-template-input-schema.json\",\n  \"title\": \"UpdateEnvironmentTemplateInput\",\n  \"description\": \"UpdateEnvironmentTemplateInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the environment template update.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The name of the environment template to update as displayed in the developer interface.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template to update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-template-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateEnvironmentTemplateInput
---
