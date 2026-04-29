---
description: CreateRecipeRequest schema from Amazon Glue DataBrew API
layout: schema
name: CreateRecipeRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Steps
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-create-recipe-request-schema.json
slug: glue-databrew-create-recipe-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-recipe-request-schema.json\",\n  \"title\": \"CreateRecipeRequest\",\n  \"description\": \"CreateRecipeRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeDescription\"\n        },\n        {\n          \"description\": \"A description for the recipe.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"A unique name for the recipe. Valid characters are alphanumeric (A-Z, a-z, 0-9), hyphen (-), period (.), and space.\"\n        }\n      ]\n    },\n    \"Steps\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/RecipeStepList\"\n        },\n        {\n          \"description\": \"An array containing the steps to be performed by the recipe. Each recipe step consists of one recipe action and (optionally) an array of condition expressions.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags to apply to this recipe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Steps\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-recipe-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CreateRecipeRequest
---
