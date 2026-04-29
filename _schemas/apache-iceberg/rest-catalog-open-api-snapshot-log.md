---
description: SnapshotLog schema from Apache Iceberg REST Catalog API
layout: schema
name: SnapshotLog
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-snapshot-log-schema.json
slug: rest-catalog-open-api-snapshot-log
source_filename: rest-catalog-open-api-snapshot-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-log-schema.json\",\n  \"title\": \"SnapshotLog\",\n  \"description\": \"SnapshotLog schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"snapshot-id\",\n      \"timestamp-ms\"\n    ],\n    \"properties\": {\n      \"snapshot-id\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"timestamp-ms\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-log-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SnapshotLog
---
