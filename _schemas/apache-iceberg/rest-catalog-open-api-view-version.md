---
description: ViewVersion schema from Apache Iceberg REST Catalog API
layout: schema
name: ViewVersion
properties_list:
- description: ''
  name: version-id
  type: integer
- description: ''
  name: timestamp-ms
  type: integer
- description: Schema ID to set as current, or -1 to set last added schema
  name: schema-id
  type: integer
- description: ''
  name: summary
  type: object
- description: ''
  name: representations
  type: array
- description: ''
  name: default-catalog
  type: string
- description: ''
  name: default-namespace
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-view-version-schema.json
slug: rest-catalog-open-api-view-version
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ViewVersion
---
