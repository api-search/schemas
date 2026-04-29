---
description: The table's last assigned partition id must match the requirement's `last-assigned-partition-id`
layout: schema
name: AssertLastAssignedPartitionId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: last-assigned-partition-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-last-assigned-partition-id-schema.json
slug: rest-catalog-open-api-assert-last-assigned-partition-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-last-assigned-partition-id-schema.json\",\n  \"title\": \"AssertLastAssignedPartitionId\",\n  \"description\": \"The table's last assigned partition id must match the requirement's `last-assigned-partition-id`\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-last-assigned-partition-id\"\n    },\n    \"last-assigned-partition-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"last-assigned-partition-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-last-assigned-partition-id-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertLastAssignedPartitionId
---
