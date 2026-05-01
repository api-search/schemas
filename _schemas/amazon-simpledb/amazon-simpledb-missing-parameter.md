---
description: The request must contain the specified missing parameter.
layout: schema
name: MissingParameter
properties_list:
- description: ''
  name: BoxUsage
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-missing-parameter-schema.json
slug: amazon-simpledb-missing-parameter
source_filename: amazon-simpledb-missing-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-missing-parameter-schema.json\",\n  \"title\": \"MissingParameter\",\n  \"description\": \"The request must contain the specified missing parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BoxUsage\": {\n      \"$ref\": \"#/components/schemas/Float\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-missing-parameter-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: MissingParameter
---
