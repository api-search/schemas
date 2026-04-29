---
description: PlanTableScanRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: PlanTableScanRequest
properties_list:
- description: Identifier for the snapshot to scan in a point-in-time scan
  name: snapshot-id
  type: integer
- description: List of selected schema fields
  name: select
  type: array
- description: Expression used to filter the table data
  name: filter
  type: object
- description: The minimum number of rows requested for the scan. This is used as a hint to the server to not have to return more rows than necessary. It is not required for the server to return that many rows since
  name: min-rows-requested
  type: integer
- description: Enables case sensitive field matching for filter and select
  name: case-sensitive
  type: boolean
- description: Whether to use the schema at the time the snapshot was written. When time travelling, the snapshot schema should be used (true). When scanning a branch, the table schema should be used (false).
  name: use-snapshot-schema
  type: boolean
- description: Starting snapshot ID for an incremental scan (exclusive)
  name: start-snapshot-id
  type: integer
- description: Ending snapshot ID for an incremental scan (inclusive). Required when start-snapshot-id is specified.
  name: end-snapshot-id
  type: integer
- description: List of fields for which the service should send column stats.
  name: stats-fields
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-plan-table-scan-request-schema.json
slug: rest-catalog-open-api-plan-table-scan-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-plan-table-scan-request-schema.json\",\n  \"title\": \"PlanTableScanRequest\",\n  \"description\": \"PlanTableScanRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"snapshot-id\": {\n      \"description\": \"Identifier for the snapshot to scan in a point-in-time scan\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"select\": {\n      \"description\": \"List of selected schema fields\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FieldName\"\n      }\n    },\n    \"filter\": {\n      \"description\": \"Expression used to filter the table data\",\n      \"$ref\": \"#/components/schemas/Expression\"\n    },\n    \"min-rows-requested\": {\n      \"description\"\
  : \"The minimum number of rows requested for the scan. This is used as a hint to the server to not have to return more rows than necessary. It is not required for the server to return that many rows since the scan may not produce that many rows. The server can also return more rows than requested.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"case-sensitive\": {\n      \"description\": \"Enables case sensitive field matching for filter and select\",\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"use-snapshot-schema\": {\n      \"description\": \"Whether to use the schema at the time the snapshot was written.\\nWhen time travelling, the snapshot schema should be used (true). When scanning a branch, the table schema should be used (false).\",\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"start-snapshot-id\": {\n      \"description\": \"Starting snapshot ID for an incremental scan (exclusive)\",\n      \"type\"\
  : \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-snapshot-id\": {\n      \"description\": \"Ending snapshot ID for an incremental scan (inclusive).\\nRequired when start-snapshot-id is specified.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"stats-fields\": {\n      \"description\": \"List of fields for which the service should send column stats.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FieldName\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-plan-table-scan-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PlanTableScanRequest
---
