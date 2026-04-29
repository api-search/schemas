---
description: ListRecipesResponse schema from Amazon Glue DataBrew API
layout: schema
name: ListRecipesResponse
properties_list:
- description: ''
  name: Recipes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-list-recipes-response-schema.json
slug: glue-databrew-list-recipes-response
source_filename: glue-databrew-list-recipes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-recipes-response-schema.json\",\n  \"title\": \"ListRecipesResponse\",\n  \"description\": \"ListRecipesResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Recipes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeList\"\n        },\n        {\n          \"description\": \"A list of recipes that are defined.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that you can use in a subsequent call to retrieve the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Recipes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-recipes-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ListRecipesResponse
---
