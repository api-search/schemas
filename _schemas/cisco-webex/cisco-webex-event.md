---
description: Represents an activity event within a Webex organization, used for compliance and auditing purposes.
layout: schema
name: Cisco Webex Event
properties_list:
- description: Unique identifier for the event.
  name: id
  type: string
- description: The resource type affected by the event.
  name: resource
  type: string
- description: The type of event that occurred.
  name: type
  type: string
- description: The application ID that triggered the event.
  name: appId
  type: string
- description: The person ID who performed the action.
  name: actorId
  type: string
- description: The organization ID where the event occurred.
  name: orgId
  type: string
- description: Date and time the event occurred.
  name: created
  type: string
- description: The resource data at the time of the event.
  name: data
  type: object
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-event-schema.json
slug: cisco-webex-event
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Event
---
