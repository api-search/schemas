---
description: ScanReport schema from Apache Iceberg REST Catalog API
layout: schema
name: ScanReport
properties_list:
- description: ''
  name: table-name
  type: string
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: filter
  type: object
- description: ''
  name: schema-id
  type: integer
- description: ''
  name: projected-field-ids
  type: array
- description: ''
  name: projected-field-names
  type: array
- description: ''
  name: metrics
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-scan-report-schema.json
slug: rest-catalog-open-api-scan-report
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ScanReport
---
