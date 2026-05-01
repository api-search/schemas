---
description: UpdateProjectResponse schema from Amazon Glue DataBrew API
layout: schema
name: UpdateProjectResponse
properties_list:
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-project-response-schema.json
slug: glue-databrew-update-project-response
source_filename: glue-databrew-update-project-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-project-response-schema.json\",\n  \"title\": \"UpdateProjectResponse\",\n  \"description\": \"UpdateProjectResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the project was last modified.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that you updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-project-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateProjectResponse
---
