---
description: A timeout occurred when attempting to query the specified domain with specified query expression.
layout: schema
name: RequestTimeout
properties_list:
- description: ''
  name: BoxUsage
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-request-timeout-schema.json
slug: amazon-simpledb-request-timeout
source_filename: amazon-simpledb-request-timeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-request-timeout-schema.json\",\n  \"title\": \"RequestTimeout\",\n  \"description\": \"A timeout occurred when attempting to query the specified domain with specified query expression.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BoxUsage\": {\n      \"$ref\": \"#/components/schemas/Float\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-request-timeout-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: RequestTimeout
---
