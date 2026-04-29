---
description: GetServiceTemplateVersionOutput schema from Amazon Proton API
layout: schema
name: GetServiceTemplateVersionOutput
properties_list:
- description: ''
  name: serviceTemplateVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-template-version-output-schema.json
slug: amazon-proton-get-service-template-version-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-template-version-output-schema.json\",\n  \"title\": \"GetServiceTemplateVersionOutput\",\n  \"description\": \"GetServiceTemplateVersionOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceTemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateVersion\"\n        },\n        {\n          \"description\": \"The detailed data of the requested service template version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceTemplateVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-template-version-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceTemplateVersionOutput
---
