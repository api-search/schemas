---
description: ListRecipeVersionsResponse schema from Amazon Glue DataBrew API
layout: schema
name: ListRecipeVersionsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Recipes
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-list-recipe-versions-response-schema.json
slug: glue-databrew-list-recipe-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-recipe-versions-response-schema.json\",\n  \"title\": \"ListRecipeVersionsResponse\",\n  \"description\": \"ListRecipeVersionsResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that you can use in a subsequent call to retrieve the next set of results.\"\n        }\n      ]\n    },\n    \"Recipes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeList\"\n        },\n        {\n          \"description\": \"A list of versions for the specified recipe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Recipes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-recipe-versions-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ListRecipeVersionsResponse
---
