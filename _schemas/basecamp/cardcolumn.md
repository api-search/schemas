---
description: A column within a card table
layout: schema
name: CardColumn
properties_list:
- description: Column ID
  name: id
  type: integer
- description: Column title
  name: title
  type: string
- description: Column type (Kanban::Column, Kanban::Triage, etc.)
  name: type
  type: string
- description: Column color
  name: color
  type: string
- description: Column position within the table
  name: position
  type: integer
- description: Number of cards in this column
  name: cards_count
  type: integer
- description: API URL to list cards in this column
  name: cards_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/cardcolumn-schema.json
slug: cardcolumn
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CardColumn
---
