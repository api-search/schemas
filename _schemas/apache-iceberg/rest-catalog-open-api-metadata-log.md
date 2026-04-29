---
description: MetadataLog schema from Apache Iceberg REST Catalog API
layout: schema
name: MetadataLog
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-metadata-log-schema.json
slug: rest-catalog-open-api-metadata-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metadata-log-schema.json\",\n  \"title\": \"MetadataLog\",\n  \"description\": \"MetadataLog schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"metadata-file\",\n      \"timestamp-ms\"\n    ],\n    \"properties\": {\n      \"metadata-file\": {\n        \"type\": \"string\"\n      },\n      \"timestamp-ms\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metadata-log-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: MetadataLog
---
