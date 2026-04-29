---
description: ViewHistoryEntry schema from Apache Iceberg REST Catalog API
layout: schema
name: ViewHistoryEntry
properties_list:
- description: ''
  name: version-id
  type: integer
- description: ''
  name: timestamp-ms
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-view-history-entry-schema.json
slug: rest-catalog-open-api-view-history-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-history-entry-schema.json\",\n  \"title\": \"ViewHistoryEntry\",\n  \"description\": \"ViewHistoryEntry schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version-id\": {\n      \"type\": \"integer\"\n    },\n    \"timestamp-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"version-id\",\n    \"timestamp-ms\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-history-entry-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ViewHistoryEntry
---
