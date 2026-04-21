---
description: ContentFile schema from Apache Iceberg REST Catalog API
layout: schema
name: ContentFile
properties_list:
- description: ''
  name: content
  type: string
- description: ''
  name: file-path
  type: string
- description: ''
  name: file-format
  type: object
- description: ''
  name: spec-id
  type: integer
- description: A list of partition field values ordered based on the fields of the partition spec specified by the `spec-id`
  name: partition
  type: array
- description: Total file size in bytes
  name: file-size-in-bytes
  type: integer
- description: Number of records in the file
  name: record-count
  type: integer
- description: Encryption key metadata blob
  name: key-metadata
  type: object
- description: List of splittable offsets
  name: split-offsets
  type: array
- description: ''
  name: sort-order-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-content-file-schema.json
slug: rest-catalog-open-api-content-file
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ContentFile
---
