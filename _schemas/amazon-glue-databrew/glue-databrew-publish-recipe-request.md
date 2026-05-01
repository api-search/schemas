---
description: PublishRecipeRequest schema from Amazon Glue DataBrew API
layout: schema
name: PublishRecipeRequest
properties_list:
- description: ''
  name: Description
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-publish-recipe-request-schema.json
slug: glue-databrew-publish-recipe-request
source_filename: glue-databrew-publish-recipe-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-publish-recipe-request-schema.json\",\n  \"title\": \"PublishRecipeRequest\",\n  \"description\": \"PublishRecipeRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeDescription\"\n        },\n        {\n          \"description\": \"A description of the recipe to be published, for this version of the recipe.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-publish-recipe-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: PublishRecipeRequest
---
