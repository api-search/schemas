---
description: Represents a set of options that define the structure of either comma-separated value (CSV), Excel, or JSON input.
layout: schema
name: FormatOptions
properties_list:
- description: ''
  name: Json
  type: object
- description: ''
  name: Excel
  type: object
- description: ''
  name: Csv
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-format-options-schema.json
slug: glue-databrew-format-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-format-options-schema.json\",\n  \"title\": \"FormatOptions\",\n  \"description\": \"Represents a set of options that define the structure of either comma-separated value (CSV), Excel, or JSON input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Json\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonOptions\"\n        },\n        {\n          \"description\": \"Options that define how JSON input is to be interpreted by DataBrew.\"\n        }\n      ]\n    },\n    \"Excel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExcelOptions\"\n        },\n        {\n          \"description\": \"Options that define how Excel input is to be interpreted by DataBrew.\"\n        }\n      ]\n    },\n    \"Csv\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CsvOptions\"\n        },\n        {\n          \"description\": \"Options that define how CSV input is to be interpreted by DataBrew.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-format-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: FormatOptions
---
