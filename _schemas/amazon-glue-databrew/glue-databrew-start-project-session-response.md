---
description: StartProjectSessionResponse schema from Amazon Glue DataBrew API
layout: schema
name: StartProjectSessionResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ClientSessionId
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-start-project-session-response-schema.json
slug: glue-databrew-start-project-session-response
source_filename: glue-databrew-start-project-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-project-session-response-schema.json\",\n  \"title\": \"StartProjectSessionResponse\",\n  \"description\": \"StartProjectSessionResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project to be acted upon.\"\n        }\n      ]\n    },\n    \"ClientSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientSessionId\"\n        },\n        {\n          \"description\": \"A system-generated identifier for the session.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-project-session-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StartProjectSessionResponse
---
