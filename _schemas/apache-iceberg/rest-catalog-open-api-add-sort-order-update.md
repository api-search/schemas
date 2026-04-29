---
description: AddSortOrderUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: AddSortOrderUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: sort-order
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-add-sort-order-update-schema.json
slug: rest-catalog-open-api-add-sort-order-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-sort-order-update-schema.json\",\n  \"title\": \"AddSortOrderUpdate\",\n  \"description\": \"AddSortOrderUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"add-sort-order\"\n    },\n    \"sort-order\": {\n      \"$ref\": \"#/components/schemas/SortOrder\"\n    }\n  },\n  \"required\": [\n    \"sort-order\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-sort-order-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AddSortOrderUpdate
---
