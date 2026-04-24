---
description: ''
layout: schema
name: CardMoveRequest
properties_list:
- description: Recording ID of the card to move
  name: source_id
  type: integer
- description: Recording ID of the destination column
  name: target_id
  type: integer
- description: Zero-indexed position within the destination column
  name: position
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/cardmoverequest-schema.json
slug: cardmoverequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CardMoveRequest
---
