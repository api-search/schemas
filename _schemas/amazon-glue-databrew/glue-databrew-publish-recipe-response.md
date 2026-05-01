---
description: PublishRecipeResponse schema from Amazon Glue DataBrew API
layout: schema
name: PublishRecipeResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-publish-recipe-response-schema.json
slug: glue-databrew-publish-recipe-response
source_filename: glue-databrew-publish-recipe-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-publish-recipe-response-schema.json\",\n  \"title\": \"PublishRecipeResponse\",\n  \"description\": \"PublishRecipeResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of the recipe that you published.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-publish-recipe-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: PublishRecipeResponse
---
