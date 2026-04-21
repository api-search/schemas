---
description: Request body for exporting an Apple Keynote presentation
layout: schema
name: ExportRequest
properties_list:
- description: Export format
  name: format
  type: string
- description: Whether to include presenter notes
  name: includeNotes
  type: boolean
- description: Slide range to export (e.g. 1-5,8)
  name: slideRange
  type: string
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-export-request-schema.json
slug: apple-keynote-export-request
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: ExportRequest
---
