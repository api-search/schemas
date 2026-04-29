---
description: The table's current schema id must match the requirement's `current-schema-id`
layout: schema
name: AssertCurrentSchemaId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: current-schema-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-current-schema-id-schema.json
slug: rest-catalog-open-api-assert-current-schema-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-current-schema-id-schema.json\",\n  \"title\": \"AssertCurrentSchemaId\",\n  \"description\": \"The table's current schema id must match the requirement's `current-schema-id`\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-current-schema-id\"\n    },\n    \"current-schema-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"current-schema-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-current-schema-id-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertCurrentSchemaId
---
