---
description: Request to evaluate a mapping template
layout: schema
name: EvaluateMappingTemplateRequest
properties_list:
- description: The mapping template to evaluate
  name: template
  type: string
- description: The template context as a JSON string
  name: context
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-evaluate-mapping-template-request-schema.json
slug: appsync-evaluate-mapping-template-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-evaluate-mapping-template-request-schema.json\",\n  \"title\": \"EvaluateMappingTemplateRequest\",\n  \"description\": \"Request to evaluate a mapping template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"template\": {\n      \"type\": \"string\",\n      \"description\": \"The mapping template to evaluate\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The template context as a JSON string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-evaluate-mapping-template-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: EvaluateMappingTemplateRequest
---
