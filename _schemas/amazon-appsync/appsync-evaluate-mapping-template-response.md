---
description: Response from evaluating a mapping template
layout: schema
name: EvaluateMappingTemplateResponse
properties_list:
- description: The evaluated template result
  name: evaluationResult
  type: string
- description: Error from template evaluation if any
  name: error
  type: object
- description: Evaluation log messages
  name: logs
  type: array
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-evaluate-mapping-template-response-schema.json
slug: appsync-evaluate-mapping-template-response
source_filename: appsync-evaluate-mapping-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-evaluate-mapping-template-response-schema.json\",\n  \"title\": \"EvaluateMappingTemplateResponse\",\n  \"description\": \"Response from evaluating a mapping template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"evaluationResult\": {\n      \"type\": \"string\",\n      \"description\": \"The evaluated template result\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error from template evaluation if any\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Evaluation log messages\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-evaluate-mapping-template-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: EvaluateMappingTemplateResponse
---
