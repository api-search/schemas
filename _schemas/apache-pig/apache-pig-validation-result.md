---
description: ValidationResult schema from Apache Pig
layout: schema
name: ValidationResult
properties_list:
- description: ''
  name: valid
  type: boolean
- description: ''
  name: errors
  type: array
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-validation-result-schema.json
slug: apache-pig-validation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-validation-result-schema.json\",\n  \"title\": \"ValidationResult\",\n  \"description\": \"ValidationResult schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ValidationError\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-validation-result-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: ValidationResult
---
