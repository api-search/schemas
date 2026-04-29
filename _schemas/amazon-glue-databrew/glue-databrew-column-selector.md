---
description: Selector of a column from a dataset for profile job configuration. One selector includes either a column name or a regular expression.
layout: schema
name: ColumnSelector
properties_list:
- description: ''
  name: Regex
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-column-selector-schema.json
slug: glue-databrew-column-selector
source_filename: glue-databrew-column-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-column-selector-schema.json\",\n  \"title\": \"ColumnSelector\",\n  \"description\": \"Selector of a column from a dataset for profile job configuration. One selector includes either a column name or a regular expression.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"A regular expression for selecting a column from a dataset.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of a column from a dataset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-column-selector-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ColumnSelector
---
