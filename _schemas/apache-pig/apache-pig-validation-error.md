---
description: ValidationError schema from Apache Pig
layout: schema
name: ValidationError
properties_list:
- description: ''
  name: line
  type: integer
- description: ''
  name: column
  type: integer
- description: ''
  name: message
  type: string
- description: ''
  name: severity
  type: string
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-validation-error-schema.json
slug: apache-pig-validation-error
source_filename: apache-pig-validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-validation-error-schema.json\",\n  \"title\": \"ValidationError\",\n  \"description\": \"ValidationError schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"column\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Undefined alias: UNDEFINED_ALIAS\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"error\",\n        \"warning\"\n      ],\n      \"example\": \"error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-validation-error-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: ValidationError
---
