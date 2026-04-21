---
description: SetStatisticsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetStatisticsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: This optional field is **DEPRECATED for REMOVAL** since it contains redundant information. Clients should use the `statistics.snapshot-id` field instead.
  name: snapshot-id
  type: integer
- description: ''
  name: statistics
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-statistics-update-schema.json
slug: rest-catalog-open-api-set-statistics-update
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetStatisticsUpdate
---
