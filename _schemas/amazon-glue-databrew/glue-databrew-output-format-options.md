---
description: Represents a set of options that define the structure of comma-separated (CSV) job output.
layout: schema
name: OutputFormatOptions
properties_list:
- description: ''
  name: Csv
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-output-format-options-schema.json
slug: glue-databrew-output-format-options
source_filename: glue-databrew-output-format-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-output-format-options-schema.json\",\n  \"title\": \"OutputFormatOptions\",\n  \"description\": \"Represents a set of options that define the structure of comma-separated (CSV) job output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Csv\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CsvOutputOptions\"\n        },\n        {\n          \"description\": \"Represents a set of options that define the structure of comma-separated value (CSV) job output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-output-format-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: OutputFormatOptions
---
