---
description: Represents a webhook registration that receives real-time HTTP callbacks when specific events occur in Webex.
layout: schema
name: Cisco Webex Webhook
properties_list:
- description: Unique identifier for the webhook.
  name: id
  type: string
- description: A user-friendly name for the webhook.
  name: name
  type: string
- description: The URL that receives webhook POST requests.
  name: targetUrl
  type: string
- description: The resource type monitored by the webhook.
  name: resource
  type: string
- description: The event type monitored by the webhook.
  name: event
  type: string
- description: The filter expression for narrowing webhook scope.
  name: filter
  type: string
- description: Secret used for generating payload signatures for verification.
  name: secret
  type: string
- description: The current status of the webhook.
  name: status
  type: string
- description: Webhook ownership type.
  name: ownedBy
  type: string
- description: Organization ID of the webhook owner.
  name: orgId
  type: string
- description: Person ID of the webhook creator.
  name: createdBy
  type: string
- description: Application ID associated with the webhook.
  name: appId
  type: string
- description: Date and time the webhook was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-webhook-schema.json
slug: cisco-webex-webhook
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Webhook
---
