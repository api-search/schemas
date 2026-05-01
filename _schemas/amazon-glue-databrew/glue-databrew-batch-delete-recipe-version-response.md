---
description: BatchDeleteRecipeVersionResponse schema from Amazon Glue DataBrew API
layout: schema
name: BatchDeleteRecipeVersionResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-batch-delete-recipe-version-response-schema.json
slug: glue-databrew-batch-delete-recipe-version-response
source_filename: glue-databrew-batch-delete-recipe-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-batch-delete-recipe-version-response-schema.json\",\n  \"title\": \"BatchDeleteRecipeVersionResponse\",\n  \"description\": \"BatchDeleteRecipeVersionResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of the recipe that was modified.\"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeErrorList\"\n        },\n        {\n          \"description\": \"Errors, if any, that occurred while attempting to delete the recipe versions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-batch-delete-recipe-version-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: BatchDeleteRecipeVersionResponse
---
