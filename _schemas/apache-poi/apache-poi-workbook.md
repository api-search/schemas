---
description: Excel workbook metadata
layout: schema
name: Workbook
properties_list:
- description: Workbook identifier
  name: id
  type: string
- description: Workbook filename
  name: name
  type: string
- description: Office format (legacy XLS or modern XLSX)
  name: format
  type: string
- description: Number of sheets in the workbook
  name: sheetCount
  type: integer
- description: Creation timestamp
  name: createdAt
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-workbook-schema.json
slug: apache-poi-workbook
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Workbook
---
