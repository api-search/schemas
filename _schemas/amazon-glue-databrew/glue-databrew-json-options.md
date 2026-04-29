---
description: Represents the JSON-specific options that define how input is to be interpreted by Glue DataBrew.
layout: schema
name: JsonOptions
properties_list:
- description: ''
  name: MultiLine
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-json-options-schema.json
slug: glue-databrew-json-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-json-options-schema.json\",\n  \"title\": \"JsonOptions\",\n  \"description\": \"Represents the JSON-specific options that define how input is to be interpreted by Glue DataBrew.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiLine\"\n        },\n        {\n          \"description\": \"A value that specifies whether JSON input contains embedded new line characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-json-options-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: JsonOptions
---
