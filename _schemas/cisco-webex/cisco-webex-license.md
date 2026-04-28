---
description: Represents a Webex license for an organization, including total and consumed units and subscription details.
layout: schema
name: Cisco Webex License
properties_list:
- description: Unique identifier for the license.
  name: id
  type: string
- description: Name of the license.
  name: name
  type: string
- description: Total number of license units available.
  name: totalUnits
  type: integer
- description: Number of license units consumed.
  name: consumedUnits
  type: integer
- description: Number of units consumed by users.
  name: consumedByUsers
  type: integer
- description: Number of units consumed by workspaces.
  name: consumedByWorkspaces
  type: integer
- description: Subscription ID associated with the license.
  name: subscriptionId
  type: string
- description: Webex site URL for the license.
  name: siteUrl
  type: string
- description: Type of the Webex site.
  name: siteType
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-license-schema.json
slug: cisco-webex-license
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex License
---
