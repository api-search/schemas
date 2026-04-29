---
description: A search filter for environment templates.
layout: schema
name: EnvironmentTemplateFilter
properties_list:
- description: ''
  name: majorVersion
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-environment-template-filter-schema.json
slug: amazon-proton-environment-template-filter
source_filename: amazon-proton-environment-template-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-filter-schema.json\",\n  \"title\": \"EnvironmentTemplateFilter\",\n  \"description\": \"A search filter for environment templates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"Include <code>majorVersion</code> to filter search for a major version.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"Include <code>templateName</code> to filter search for a template name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"majorVersion\",\n   \
  \ \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-filter-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: EnvironmentTemplateFilter
---
