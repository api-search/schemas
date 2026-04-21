---
description: Represents a webhook event payload delivered by the Autodesk Webhooks API to registered callback URLs when events occur in Data Management, Model Derivative, or other Autodesk systems.
layout: schema
name: Autodesk Webhook Event
properties_list:
- description: The webhook payload schema version.
  name: version
  type: string
- description: The URN of the affected resource.
  name: resourceUrn
  type: string
- description: Information about the webhook subscription that triggered this event.
  name: hook
  type: object
- description: The event-specific payload data.
  name: payload
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-webhook-event.json
slug: autodesk-webhook-event
tags:
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
title: Autodesk Webhook Event
---
