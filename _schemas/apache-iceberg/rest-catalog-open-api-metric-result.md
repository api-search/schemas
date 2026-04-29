---
description: MetricResult schema from Apache Iceberg REST Catalog API
layout: schema
name: MetricResult
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-metric-result-schema.json
slug: rest-catalog-open-api-metric-result
source_filename: rest-catalog-open-api-metric-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metric-result-schema.json\",\n  \"title\": \"MetricResult\",\n  \"description\": \"MetricResult schema from Apache Iceberg REST Catalog API\",\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/CounterResult\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/TimerResult\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-metric-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: MetricResult
---
