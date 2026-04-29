---
description: Represents a set of options that define how DataBrew will write a comma-separated value (CSV) file.
layout: schema
name: CsvOutputOptions
properties_list:
- description: ''
  name: Delimiter
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-csv-output-options-schema.json
slug: glue-databrew-csv-output-options
source_filename: glue-databrew-csv-output-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-csv-output-options-schema.json\",\n  \"title\": \"CsvOutputOptions\",\n  \"description\": \"Represents a set of options that define how DataBrew will write a comma-separated value (CSV) file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Delimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Delimiter\"\n        },\n        {\n          \"description\": \"A single character that specifies the delimiter used to create CSV job output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-csv-output-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CsvOutputOptions
---
