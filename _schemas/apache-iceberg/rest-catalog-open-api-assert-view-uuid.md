---
description: The view UUID must match the requirement's `uuid`
layout: schema
name: AssertViewUUID
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: uuid
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-view-uuid-schema.json
slug: rest-catalog-open-api-assert-view-uuid
source_filename: rest-catalog-open-api-assert-view-uuid-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-view-uuid-schema.json\",\n  \"title\": \"AssertViewUUID\",\n  \"description\": \"The view UUID must match the requirement's `uuid`\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-view-uuid\"\n    },\n    \"uuid\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"uuid\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-view-uuid-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertViewUUID
---
