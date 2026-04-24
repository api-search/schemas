---
description: A tool available on a project's dock
layout: schema
name: DockItem
properties_list:
- description: Dock item ID
  name: id
  type: integer
- description: Display title of the tool
  name: title
  type: string
- description: Internal name of the tool (e.g., message_board, todoset)
  name: name
  type: string
- description: Whether this tool is enabled on the project
  name: enabled
  type: boolean
- description: Display position of the tool in the dock
  name: position
  type: integer
- description: API URL for this tool's resource
  name: url
  type: string
- description: Web URL for this tool's resource
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/dockitem-schema.json
slug: dockitem
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: DockItem
---
