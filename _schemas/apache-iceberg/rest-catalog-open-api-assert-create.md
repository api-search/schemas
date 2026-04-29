---
description: The table must not already exist; used for create transactions
layout: schema
name: AssertCreate
properties_list:
- description: ''
  name: type
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-create-schema.json
slug: rest-catalog-open-api-assert-create
source_filename: rest-catalog-open-api-assert-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-create-schema.json\",\n  \"title\": \"AssertCreate\",\n  \"description\": \"The table must not already exist; used for create transactions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-create\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-create-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertCreate
---
