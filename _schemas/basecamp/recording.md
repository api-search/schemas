---
description: A generic recording object representing any Basecamp content resource such as a message, to-do, document, comment, or upload.
layout: schema
name: Recording
properties_list:
- description: Recording ID
  name: id
  type: integer
- description: Recording status
  name: status
  type: string
- description: Whether this recording is visible to client users
  name: visible_to_clients
  type: boolean
- description: Timestamp when the recording was created
  name: created_at
  type: string
- description: Timestamp when the recording was last updated
  name: updated_at
  type: string
- description: Title or summary of the recording
  name: title
  type: string
- description: Whether this recording inherits its status from a parent
  name: inherits_status
  type: boolean
- description: Recording type (e.g., Message, Todo, Document)
  name: type
  type: string
- description: API URL for this recording
  name: url
  type: string
- description: Web URL for this recording
  name: app_url
  type: string
- description: ''
  name: bucket
  type: object
- description: ''
  name: creator
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/recording-schema.json
slug: recording
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Recording
---
