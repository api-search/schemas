---
description: FileScanTask schema from Apache Iceberg REST Catalog API
layout: schema
name: FileScanTask
properties_list:
- description: ''
  name: data-file
  type: object
- description: A list of indices in the delete files array (0-based)
  name: delete-file-references
  type: array
- description: An optional filter to be applied to rows in this file scan task. If the residual is not present, the client must produce the residual or use the original filter.
  name: residual-filter
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-file-scan-task-schema.json
slug: rest-catalog-open-api-file-scan-task
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FileScanTask
---
