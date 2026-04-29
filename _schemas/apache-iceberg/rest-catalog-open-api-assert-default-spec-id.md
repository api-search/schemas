---
description: The table's default spec id must match the requirement's `default-spec-id`
layout: schema
name: AssertDefaultSpecId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: default-spec-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-default-spec-id-schema.json
slug: rest-catalog-open-api-assert-default-spec-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-default-spec-id-schema.json\",\n  \"title\": \"AssertDefaultSpecId\",\n  \"description\": \"The table's default spec id must match the requirement's `default-spec-id`\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-default-spec-id\"\n    },\n    \"default-spec-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"default-spec-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-default-spec-id-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertDefaultSpecId
---
