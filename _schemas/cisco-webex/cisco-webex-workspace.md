---
description: Represents a physical workspace location with Webex devices, including capacity, type, calling, and calendar configurations.
layout: schema
name: Cisco Webex Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Organization ID the workspace belongs to.
  name: orgId
  type: string
- description: Display name of the workspace.
  name: displayName
  type: string
- description: Location ID of the workspace.
  name: workspaceLocationId
  type: string
- description: Floor ID within the location.
  name: floorId
  type: string
- description: Number of people the workspace can accommodate.
  name: capacity
  type: integer
- description: Type of workspace.
  name: type
  type: string
- description: SIP address assigned to the workspace.
  name: sipAddress
  type: string
- description: Calling configuration for the workspace.
  name: calling
  type: object
- description: Calendar configuration for the workspace.
  name: calendar
  type: object
- description: Notes or description for the workspace.
  name: notes
  type: string
- description: Date and time the workspace was created.
  name: created
  type: string
- description: Date and time the workspace was last modified.
  name: lastModified
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-workspace-schema.json
slug: cisco-webex-workspace
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Workspace
---
