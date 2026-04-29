---
description: Represents a set of options that define how DataBrew selects files for a given Amazon S3 path in a dataset.
layout: schema
name: PathOptions
properties_list:
- description: ''
  name: LastModifiedDateCondition
  type: object
- description: ''
  name: FilesLimit
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-path-options-schema.json
slug: glue-databrew-path-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-path-options-schema.json\",\n  \"title\": \"PathOptions\",\n  \"description\": \"Represents a set of options that define how DataBrew selects files for a given Amazon S3 path in a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LastModifiedDateCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterExpression\"\n        },\n        {\n          \"description\": \"If provided, this structure defines a date range for matching Amazon S3 objects based on their LastModifiedDate attribute in Amazon S3.\"\n        }\n      ]\n    },\n    \"FilesLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilesLimit\"\n        },\n        {\n          \"description\": \"If provided, this structure imposes a limit\
  \ on a number of files that should be selected.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathParametersMap\"\n        },\n        {\n          \"description\": \"A structure that maps names of parameters used in the Amazon S3 path of a dataset to their definitions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-path-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: PathOptions
---
