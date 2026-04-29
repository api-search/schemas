---
description: Represents the name and version of a DataBrew recipe.
layout: schema
name: RecipeReference
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RecipeVersion
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-recipe-reference-schema.json
slug: glue-databrew-recipe-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-reference-schema.json\",\n  \"title\": \"RecipeReference\",\n  \"description\": \"Represents the name and version of a DataBrew recipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of the recipe.\"\n        }\n      ]\n    },\n    \"RecipeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeVersion\"\n        },\n        {\n          \"description\": \"The identifier for the version for the recipe. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-reference-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: RecipeReference
---
