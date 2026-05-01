---
description: UpdateProjectRequest schema from Amazon Glue DataBrew API
layout: schema
name: UpdateProjectRequest
properties_list:
- description: ''
  name: Sample
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-project-request-schema.json
slug: glue-databrew-update-project-request
source_filename: glue-databrew-update-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-project-request-schema.json\",\n  \"title\": \"UpdateProjectRequest\",\n  \"description\": \"UpdateProjectRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sample\": {\n      \"$ref\": \"#/components/schemas/Sample\"\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role to be assumed for this request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-project-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateProjectRequest
---
