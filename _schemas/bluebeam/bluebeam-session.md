---
description: JSON Schema for a Bluebeam Studio Session used for collaborative PDF document review and markup.
layout: schema
name: Bluebeam Studio Session
properties_list:
- description: Unique Studio Session identifier
  name: id
  type: string
- description: Session display name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: status
  type: string
- description: URL users can use to join the session
  name: inviteUrl
  type: string
- description: Default permission level for new attendees
  name: defaultPermission
  type: string
- description: Whether attendees can invite others
  name: allowInvitations
  type: boolean
- description: Whether the session requires explicit invitation
  name: restricted
  type: boolean
- description: User who created the session
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: ''
  name: documentCount
  type: integer
- description: ''
  name: userCount
  type: integer
provider_name: bluebeam
provider_slug: bluebeam
schema_file: json-schema/bluebeam-session-schema.json
slug: bluebeam-session
tags: []
title: Bluebeam Studio Session
---
