---
description: CreateServiceTemplateVersionOutput schema from Amazon Proton API
layout: schema
name: CreateServiceTemplateVersionOutput
properties_list:
- description: ''
  name: serviceTemplateVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-template-version-output-schema.json
slug: amazon-proton-create-service-template-version-output
source_filename: amazon-proton-create-service-template-version-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-version-output-schema.json\",\n  \"title\": \"CreateServiceTemplateVersionOutput\",\n  \"description\": \"CreateServiceTemplateVersionOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceTemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateVersion\"\n        },\n        {\n          \"description\": \"The service template version summary of detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceTemplateVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-version-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceTemplateVersionOutput
---
