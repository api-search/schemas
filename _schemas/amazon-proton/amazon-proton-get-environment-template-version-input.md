---
description: GetEnvironmentTemplateVersionInput schema from Amazon Proton API
layout: schema
name: GetEnvironmentTemplateVersionInput
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
schema_file: json-schema/amazon-proton-get-environment-template-version-input-schema.json
slug: amazon-proton-get-environment-template-version-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-template-version-input-schema.json\",\n  \"title\": \"GetEnvironmentTemplateVersionInput\",\n  \"description\": \"GetEnvironmentTemplateVersionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"To get environment template major version detail data, include <code>major Version</code>.\"\n        }\n      ]\n    },\n    \"minorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"To get environment template minor version detail data, include <code>minorVersion</code>.\"\
  \n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template a version of which you want to get detailed data for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"majorVersion\",\n    \"minorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-template-version-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetEnvironmentTemplateVersionInput
---
