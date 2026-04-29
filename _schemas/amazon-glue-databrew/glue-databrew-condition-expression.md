---
description: <p>Represents an individual condition that evaluates to true or false.</p> <p>Conditions are used with recipe actions. The action is only performed for column values where the condition evaluates to true.</p> <p>If a recipe requires more than one condition, then the recipe must specify multiple <code>ConditionExpression</code> elements. Each condition is applied to the rows in a dataset first, before the recipe action is performed.</p>
layout: schema
name: ConditionExpression
properties_list:
- description: ''
  name: Condition
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: TargetColumn
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-condition-expression-schema.json
slug: glue-databrew-condition-expression
source_filename: glue-databrew-condition-expression-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-condition-expression-schema.json\",\n  \"title\": \"ConditionExpression\",\n  \"description\": \"<p>Represents an individual condition that evaluates to true or false.</p> <p>Conditions are used with recipe actions. The action is only performed for column values where the condition evaluates to true.</p> <p>If a recipe requires more than one condition, then the recipe must specify multiple <code>ConditionExpression</code> elements. Each condition is applied to the rows in a dataset first, before the recipe action is performed.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Condition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Condition\"\n        },\n        {\n          \"description\": \"A specific condition to apply to a recipe action.\
  \ For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/recipes.html#recipes.structure\\\">Recipe structure</a> in the <i>Glue DataBrew Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionValue\"\n        },\n        {\n          \"description\": \"A value that the condition must evaluate to for the condition to succeed.\"\n        }\n      ]\n    },\n    \"TargetColumn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetColumn\"\n        },\n        {\n          \"description\": \"A column to apply this condition to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Condition\",\n    \"TargetColumn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-condition-expression-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ConditionExpression
---
