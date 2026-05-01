---
description: Represents a single step from a DataBrew recipe to be performed.
layout: schema
name: RecipeStep
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: ConditionExpressions
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-recipe-step-schema.json
slug: glue-databrew-recipe-step
source_filename: glue-databrew-recipe-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-step-schema.json\",\n  \"title\": \"RecipeStep\",\n  \"description\": \"Represents a single step from a DataBrew recipe to be performed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeAction\"\n        },\n        {\n          \"description\": \"The particular action to be performed in the recipe step.\"\n        }\n      ]\n    },\n    \"ConditionExpressions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionExpressionList\"\n        },\n        {\n          \"description\": \"<p>One or more conditions that must be met for the recipe step to succeed.</p> <note> <p>All of the conditions in the array must be met. In other words, all of the\
  \ conditions must be combined using a logical AND operation.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-step-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: RecipeStep
---
