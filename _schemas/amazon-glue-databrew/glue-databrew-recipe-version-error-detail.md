---
description: Represents any errors encountered when attempting to delete multiple recipe versions.
layout: schema
name: RecipeVersionErrorDetail
properties_list:
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: RecipeVersion
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-recipe-version-error-detail-schema.json
slug: glue-databrew-recipe-version-error-detail
source_filename: glue-databrew-recipe-version-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-version-error-detail-schema.json\",\n  \"title\": \"RecipeVersionErrorDetail\",\n  \"description\": \"Represents any errors encountered when attempting to delete multiple recipe versions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"The HTTP status code for the error.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeErrorMessage\"\n        },\n        {\n          \"description\": \"The text of the error message.\"\n        }\n      ]\n    },\n    \"RecipeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeVersion\"\
  \n        },\n        {\n          \"description\": \"The identifier for the recipe version associated with this error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-version-error-detail-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: RecipeVersionErrorDetail
---
