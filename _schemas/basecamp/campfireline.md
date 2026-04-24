---
description: ''
layout: schema
name: CampfireLine
properties_list:
- description: Line ID
  name: id
  type: integer
- description: Line status
  name: status
  type: string
- description: Timestamp when the line was posted
  name: created_at
  type: string
- description: Timestamp when the line was last updated
  name: updated_at
  type: string
- description: Line title (summary)
  name: title
  type: string
- description: Plain text message content
  name: content
  type: string
- description: Line type
  name: type
  type: string
- description: ''
  name: creator
  type: object
- description: ''
  name: bucket
  type: object
- description: ''
  name: parent
  type: object
- description: Number of boosts on this line
  name: boosts_count
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/campfireline-schema.json
slug: campfireline
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CampfireLine
---
