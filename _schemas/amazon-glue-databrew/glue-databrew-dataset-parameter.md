---
description: Represents a dataset parameter that defines type and conditions for a parameter in the Amazon S3 path of the dataset.
layout: schema
name: DatasetParameter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: DatetimeOptions
  type: object
- description: ''
  name: CreateColumn
  type: object
- description: ''
  name: Filter
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-dataset-parameter-schema.json
slug: glue-databrew-dataset-parameter
source_filename: glue-databrew-dataset-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-dataset-parameter-schema.json\",\n  \"title\": \"DatasetParameter\",\n  \"description\": \"Represents a dataset parameter that defines type and conditions for a parameter in the Amazon S3 path of the dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathParameterName\"\n        },\n        {\n          \"description\": \"The name of the parameter that is used in the dataset's Amazon S3 path.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterType\"\n        },\n        {\n          \"description\": \"The type of the dataset parameter, can be one of a 'String', 'Number' or 'Datetime'.\"\n        }\n      ]\n\
  \    },\n    \"DatetimeOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatetimeOptions\"\n        },\n        {\n          \"description\": \"Additional parameter options such as a format and a timezone. Required for datetime parameters.\"\n        }\n      ]\n    },\n    \"CreateColumn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateColumn\"\n        },\n        {\n          \"description\": \"Optional boolean value that defines whether the captured value of this parameter should be used to create a new column in a dataset.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterExpression\"\n        },\n        {\n          \"description\": \"The optional filter expression structure to apply additional matching criteria to the parameter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-dataset-parameter-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DatasetParameter
---
