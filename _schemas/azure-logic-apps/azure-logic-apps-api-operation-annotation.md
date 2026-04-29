---
description: The Api Operation Annotation.
layout: schema
name: ApiOperationAnnotation
properties_list:
- description: The family.
  name: family
  type: string
- description: The revision.
  name: revision
  type: integer
- description: ''
  name: status
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-operation-annotation-schema.json
slug: azure-logic-apps-api-operation-annotation
source_filename: azure-logic-apps-api-operation-annotation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-annotation-schema.json\",\n  \"title\": \"ApiOperationAnnotation\",\n  \"description\": \"The Api Operation Annotation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"family\": {\n      \"description\": \"The family.\",\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"description\": \"The revision.\",\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"$ref\": \"#/definitions/StatusAnnotation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-annotation-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiOperationAnnotation
---
