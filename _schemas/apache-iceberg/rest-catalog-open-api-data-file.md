---
description: DataFile schema from Apache Iceberg REST Catalog API
layout: schema
name: DataFile
properties_list:
- description: ''
  name: content
  type: string
- description: The first row ID assigned to the first row in the data file
  name: first-row-id
  type: integer
- description: Map of column id to total count, including null and NaN
  name: column-sizes
  type: object
- description: Map of column id to null value count
  name: value-counts
  type: object
- description: Map of column id to null value count
  name: null-value-counts
  type: object
- description: Map of column id to number of NaN values in the column
  name: nan-value-counts
  type: object
- description: Map of column id to lower bound primitive type values
  name: lower-bounds
  type: object
- description: Map of column id to upper bound primitive type values
  name: upper-bounds
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-data-file-schema.json
slug: rest-catalog-open-api-data-file
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: DataFile
---
