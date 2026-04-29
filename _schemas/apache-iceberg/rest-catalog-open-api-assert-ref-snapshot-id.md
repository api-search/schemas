---
description: The table branch or tag identified by the requirement's `ref` must reference the requirement's `snapshot-id`. The `snapshot-id` field is required in this object, but in the case of a `null` the ref must not already exist.
layout: schema
name: AssertRefSnapshotId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: ref
  type: string
- description: ''
  name: snapshot-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-ref-snapshot-id-schema.json
slug: rest-catalog-open-api-assert-ref-snapshot-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-ref-snapshot-id-schema.json\",\n  \"title\": \"AssertRefSnapshotId\",\n  \"description\": \"The table branch or tag identified by the requirement's `ref` must reference the requirement's `snapshot-id`.\\nThe `snapshot-id` field is required in this object, but in the case of a `null`\\nthe ref must not already exist.\\n\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"assert-ref-snapshot-id\"\n    },\n    \"ref\": {\n      \"type\": \"string\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"ref\",\n    \"snapshot-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TableRequirement\"\n    }\n  ],\n  \"type\"\
  : \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assert-ref-snapshot-id-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertRefSnapshotId
---
