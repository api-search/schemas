---
description: Represents the sample size and sampling type for DataBrew to use for interactive data analysis.
layout: schema
name: Sample
properties_list:
- description: ''
  name: Size
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-sample-schema.json
slug: glue-databrew-sample
source_filename: glue-databrew-sample-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-sample-schema.json\",\n  \"title\": \"Sample\",\n  \"description\": \"Represents the sample size and sampling type for DataBrew to use for interactive data analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleSize\"\n        },\n        {\n          \"description\": \"The number of rows in the sample.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleType\"\n        },\n        {\n          \"description\": \"The way in which DataBrew obtains rows from a dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-sample-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Sample
---
