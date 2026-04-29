---
description: Represents a transformation and associated parameters that are used to apply a change to a DataBrew dataset. For more information, see <a href="https://docs.aws.amazon.com/databrew/latest/dg/recipe-actions-reference.html">Recipe actions reference</a>.
layout: schema
name: RecipeAction
properties_list:
- description: ''
  name: Operation
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-recipe-action-schema.json
slug: glue-databrew-recipe-action
source_filename: glue-databrew-recipe-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-action-schema.json\",\n  \"title\": \"RecipeAction\",\n  \"description\": \"Represents a transformation and associated parameters that are used to apply a change to a DataBrew dataset. For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/recipe-actions-reference.html\\\">Recipe actions reference</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Operation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Operation\"\n        },\n        {\n          \"description\": \"The name of a valid DataBrew transformation to be performed on the data.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterMap\"\n        },\n        {\n \
  \         \"description\": \"Contextual parameters for the transformation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-action-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: RecipeAction
---
