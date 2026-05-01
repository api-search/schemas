---
description: UpdateRecipeJobResponse schema from Amazon Glue DataBrew API
layout: schema
name: UpdateRecipeJobResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-recipe-job-response-schema.json
slug: glue-databrew-update-recipe-job-response
source_filename: glue-databrew-update-recipe-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-recipe-job-response-schema.json\",\n  \"title\": \"UpdateRecipeJobResponse\",\n  \"description\": \"UpdateRecipeJobResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name of the job that you updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-recipe-job-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateRecipeJobResponse
---
