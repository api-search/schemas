---
description: PositionDeleteFile schema from Apache Iceberg REST Catalog API
layout: schema
name: PositionDeleteFile
properties_list:
- description: ''
  name: content
  type: string
- description: Offset within the delete file of delete content
  name: content-offset
  type: integer
- description: Length, in bytes, of the delete content; required if content-offset is present
  name: content-size-in-bytes
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-position-delete-file-schema.json
slug: rest-catalog-open-api-position-delete-file
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PositionDeleteFile
---
