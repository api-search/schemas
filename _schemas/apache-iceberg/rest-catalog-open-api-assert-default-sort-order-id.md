---
description: The table's default sort order id must match the requirement's `default-sort-order-id`
layout: schema
name: AssertDefaultSortOrderId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: default-sort-order-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-default-sort-order-id-schema.json
slug: rest-catalog-open-api-assert-default-sort-order-id
source_filename: rest-catalog-open-api-assert-default-sort-order-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-default-sort-order-id-schema.json\",\n  \"title\": \"AssertDefaultSortOrderId\",\n  \"description\": \"The table's default sort order id must match the requirement's `default-sort-order-id`\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-default-sort-order-id\"\n    },\n    \"default-sort-order-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"default-sort-order-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-default-sort-order-id-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertDefaultSortOrderId
---
