---
description: Represents a set of options that define how DataBrew will interpret a Microsoft Excel file when creating a dataset from that file.
layout: schema
name: ExcelOptions
properties_list:
- description: ''
  name: SheetNames
  type: object
- description: ''
  name: SheetIndexes
  type: object
- description: ''
  name: HeaderRow
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-excel-options-schema.json
slug: glue-databrew-excel-options
source_filename: glue-databrew-excel-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-excel-options-schema.json\",\n  \"title\": \"ExcelOptions\",\n  \"description\": \"Represents a set of options that define how DataBrew will interpret a Microsoft Excel file when creating a dataset from that file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SheetNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SheetNameList\"\n        },\n        {\n          \"description\": \"One or more named sheets in the Excel file that will be included in the dataset.\"\n        }\n      ]\n    },\n    \"SheetIndexes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SheetIndexList\"\n        },\n        {\n          \"description\": \"One or more sheet numbers in the Excel file that will be included in the dataset.\"\
  \n        }\n      ]\n    },\n    \"HeaderRow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderRow\"\n        },\n        {\n          \"description\": \"A variable that specifies whether the first row in the file is parsed as the header. If this value is false, column names are auto-generated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-excel-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ExcelOptions
---
