---
description: SendProjectSessionActionRequest schema from Amazon Glue DataBrew API
layout: schema
name: SendProjectSessionActionRequest
properties_list:
- description: ''
  name: Preview
  type: object
- description: ''
  name: RecipeStep
  type: object
- description: ''
  name: StepIndex
  type: object
- description: ''
  name: ClientSessionId
  type: object
- description: ''
  name: ViewFrame
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-send-project-session-action-request-schema.json
slug: glue-databrew-send-project-session-action-request
source_filename: glue-databrew-send-project-session-action-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-send-project-session-action-request-schema.json\",\n  \"title\": \"SendProjectSessionActionRequest\",\n  \"description\": \"SendProjectSessionActionRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Preview\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Preview\"\n        },\n        {\n          \"description\": \"If true, the result of the recipe step will be returned, but not applied.\"\n        }\n      ]\n    },\n    \"RecipeStep\": {\n      \"$ref\": \"#/components/schemas/RecipeStep\"\n    },\n    \"StepIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StepIndex\"\n        },\n        {\n          \"description\": \"The index from which to preview a step. This\
  \ index is used to preview the result of steps that have already been applied, so that the resulting view frame is from earlier in the view frame stack.\"\n        }\n      ]\n    },\n    \"ClientSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientSessionId\"\n        },\n        {\n          \"description\": \"A unique identifier for an interactive session that's currently open and ready for work. The action will be performed on this session.\"\n        }\n      ]\n    },\n    \"ViewFrame\": {\n      \"$ref\": \"#/components/schemas/ViewFrame\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-send-project-session-action-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: SendProjectSessionActionRequest
---
