---
description: SetDefaultSortOrderUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetDefaultSortOrderUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: Sort order ID to set as the default, or -1 to set last added sort order
  name: sort-order-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-default-sort-order-update-schema.json
slug: rest-catalog-open-api-set-default-sort-order-update
source_filename: rest-catalog-open-api-set-default-sort-order-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-default-sort-order-update-schema.json\",\n  \"title\": \"SetDefaultSortOrderUpdate\",\n  \"description\": \"SetDefaultSortOrderUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"set-default-sort-order\"\n    },\n    \"sort-order-id\": {\n      \"type\": \"integer\",\n      \"description\": \"Sort order ID to set as the default, or -1 to set last added sort order\"\n    }\n  },\n  \"required\": [\n    \"sort-order-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-default-sort-order-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetDefaultSortOrderUpdate
---
