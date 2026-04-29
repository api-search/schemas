---
description: ReportMetricsRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: ReportMetricsRequest
properties_list:
- description: ''
  name: report-type
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-report-metrics-request-schema.json
slug: rest-catalog-open-api-report-metrics-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-report-metrics-request-schema.json\",\n  \"title\": \"ReportMetricsRequest\",\n  \"description\": \"ReportMetricsRequest schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"report-type\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"report-type\"\n  ],\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ScanReport\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/CommitReport\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-report-metrics-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ReportMetricsRequest
---
