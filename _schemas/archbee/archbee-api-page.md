---
description: ''
layout: schema
name: Page
properties_list:
- description: Unique page identifier
  name: id
  type: string
- description: Page title
  name: title
  type: string
- description: URL-friendly page identifier
  name: slug
  type: string
- description: Page publication status
  name: status
  type: string
- description: Page content in Markdown
  name: content
  type: string
- description: Parent space identifier
  name: spaceId
  type: string
- description: Parent page identifier (if nested)
  name: parentId
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-page-schema.json
slug: archbee-api-page
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: Page
---
