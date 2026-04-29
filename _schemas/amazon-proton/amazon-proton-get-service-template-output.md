---
description: GetServiceTemplateOutput schema from Amazon Proton API
layout: schema
name: GetServiceTemplateOutput
properties_list:
- description: ''
  name: serviceTemplate
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-template-output-schema.json
slug: amazon-proton-get-service-template-output
source_filename: amazon-proton-get-service-template-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-template-output-schema.json\",\n  \"title\": \"GetServiceTemplateOutput\",\n  \"description\": \"GetServiceTemplateOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplate\"\n        },\n        {\n          \"description\": \"The detailed data of the requested service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceTemplate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-template-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceTemplateOutput
---
