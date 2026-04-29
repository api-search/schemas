---
description: DeleteEnvironmentTemplateVersionInput schema from Amazon Proton API
layout: schema
name: DeleteEnvironmentTemplateVersionInput
properties_list:
- description: ''
  name: majorVersion
  type: object
- description: ''
  name: minorVersion
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-environment-template-version-input-schema.json
slug: amazon-proton-delete-environment-template-version-input
source_filename: amazon-proton-delete-environment-template-version-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-environment-template-version-input-schema.json\",\n  \"title\": \"DeleteEnvironmentTemplateVersionInput\",\n  \"description\": \"DeleteEnvironmentTemplateVersionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The environment template major version to delete.\"\n        }\n      ]\n    },\n    \"minorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The environment template minor version to delete.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"majorVersion\",\n    \"minorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-environment-template-version-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteEnvironmentTemplateVersionInput
---
