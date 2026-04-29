---
description: Represents a set of options that define how DataBrew will read a comma-separated value (CSV) file when creating a dataset from that file.
layout: schema
name: CsvOptions
properties_list:
- description: ''
  name: Delimiter
  type: object
- description: ''
  name: HeaderRow
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-csv-options-schema.json
slug: glue-databrew-csv-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-csv-options-schema.json\",\n  \"title\": \"CsvOptions\",\n  \"description\": \"Represents a set of options that define how DataBrew will read a comma-separated value (CSV) file when creating a dataset from that file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Delimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Delimiter\"\n        },\n        {\n          \"description\": \"A single character that specifies the delimiter being used in the CSV file.\"\n        }\n      ]\n    },\n    \"HeaderRow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderRow\"\n        },\n        {\n          \"description\": \"A variable that specifies whether the first row in the file is parsed as the header. If this value\
  \ is false, column names are auto-generated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-csv-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CsvOptions
---
