---
description: The threshold used with a non-aggregate check expression. The non-aggregate check expression will be applied to each row in a specific column. Then the threshold will be used to determine whether the validation succeeds.
layout: schema
name: Threshold
properties_list:
- description: ''
  name: Value
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Unit
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-threshold-schema.json
slug: glue-databrew-threshold
source_filename: glue-databrew-threshold-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-threshold-schema.json\",\n  \"title\": \"Threshold\",\n  \"description\": \"The threshold used with a non-aggregate check expression. The non-aggregate check expression will be applied to each row in a specific column. Then the threshold will be used to determine whether the validation succeeds.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdValue\"\n        },\n        {\n          \"description\": \"The value of a threshold.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdType\"\n        },\n        {\n          \"description\": \"The type of a threshold. Used for comparison of an actual count of rows\
  \ that satisfy the rule to the threshold value.\"\n        }\n      ]\n    },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdUnit\"\n        },\n        {\n          \"description\": \"Unit of threshold value. Can be either a COUNT or PERCENTAGE of the full sample size used for validation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-threshold-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Threshold
---
