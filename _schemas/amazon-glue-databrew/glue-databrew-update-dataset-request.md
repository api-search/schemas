---
description: UpdateDatasetRequest schema from Amazon Glue DataBrew API
layout: schema
name: UpdateDatasetRequest
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: FormatOptions
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: PathOptions
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-dataset-request-schema.json
slug: glue-databrew-update-dataset-request
source_filename: glue-databrew-update-dataset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-dataset-request-schema.json\",\n  \"title\": \"UpdateDatasetRequest\",\n  \"description\": \"UpdateDatasetRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \"The file format of a dataset that is created from an Amazon S3 file or folder.\"\n        }\n      ]\n    },\n    \"FormatOptions\": {\n      \"$ref\": \"#/components/schemas/FormatOptions\"\n    },\n    \"Input\": {\n      \"$ref\": \"#/components/schemas/Input\"\n    },\n    \"PathOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathOptions\"\n        },\n        {\n          \"description\"\
  : \"A set of options that defines how DataBrew interprets an Amazon S3 path of the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Input\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-dataset-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateDatasetRequest
---
