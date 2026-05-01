---
description: SendProjectSessionActionResponse schema from Amazon Glue DataBrew API
layout: schema
name: SendProjectSessionActionResponse
properties_list:
- description: ''
  name: Result
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ActionId
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-send-project-session-action-response-schema.json
slug: glue-databrew-send-project-session-action-response
source_filename: glue-databrew-send-project-session-action-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-send-project-session-action-response-schema.json\",\n  \"title\": \"SendProjectSessionActionResponse\",\n  \"description\": \"SendProjectSessionActionResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Result\"\n        },\n        {\n          \"description\": \"A message indicating the result of performing the action.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that was affected by the action.\"\n        }\n      ]\n    },\n    \"ActionId\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/ActionId\"\n        },\n        {\n          \"description\": \"A unique identifier for the action that was performed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-send-project-session-action-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: SendProjectSessionActionResponse
---
