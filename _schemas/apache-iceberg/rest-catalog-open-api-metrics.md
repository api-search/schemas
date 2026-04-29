---
description: Metrics schema from Apache Iceberg REST Catalog API
layout: schema
name: Metrics
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-metrics-schema.json
slug: rest-catalog-open-api-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metrics-schema.json\",\n  \"title\": \"Metrics\",\n  \"description\": \"Metrics schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/MetricResult\"\n  },\n  \"example\": {\n    \"metrics\": {\n      \"total-planning-duration\": {\n        \"count\": 1,\n        \"time-unit\": \"nanoseconds\",\n        \"total-duration\": 2644235116\n      },\n      \"result-data-files\": {\n        \"unit\": \"count\",\n        \"value\": 1\n      },\n      \"result-delete-files\": {\n        \"unit\": \"count\",\n        \"value\": 0\n      },\n      \"total-data-manifests\": {\n        \"unit\": \"count\",\n        \"value\": 1\n      },\n      \"total-delete-manifests\": {\n        \"unit\": \"count\",\n    \
  \    \"value\": 0\n      },\n      \"scanned-data-manifests\": {\n        \"unit\": \"count\",\n        \"value\": 1\n      },\n      \"skipped-data-manifests\": {\n        \"unit\": \"count\",\n        \"value\": 0\n      },\n      \"total-file-size-bytes\": {\n        \"unit\": \"bytes\",\n        \"value\": 10\n      },\n      \"total-delete-file-size-bytes\": {\n        \"unit\": \"bytes\",\n        \"value\": 0\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metrics-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Metrics
---
