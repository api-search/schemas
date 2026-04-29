---
description: AddSnapshotUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: AddSnapshotUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: snapshot
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-add-snapshot-update-schema.json
slug: rest-catalog-open-api-add-snapshot-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-snapshot-update-schema.json\",\n  \"title\": \"AddSnapshotUpdate\",\n  \"description\": \"AddSnapshotUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"add-snapshot\"\n    },\n    \"snapshot\": {\n      \"$ref\": \"#/components/schemas/Snapshot\"\n    }\n  },\n  \"required\": [\n    \"snapshot\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-snapshot-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AddSnapshotUpdate
---
