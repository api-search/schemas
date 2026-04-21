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
