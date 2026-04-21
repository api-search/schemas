---
description: Request to create an Excel workbook
layout: schema
name: WorkbookRequest
properties_list:
- description: Workbook filename
  name: name
  type: string
- description: Output format
  name: format
  type: string
- description: Initial sheet names
  name: sheets
  type: array
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-workbook-request-schema.json
slug: apache-poi-workbook-request
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: WorkbookRequest
---
