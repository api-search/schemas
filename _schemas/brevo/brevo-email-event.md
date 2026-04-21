---
description: Represents a webhook event payload delivered by Brevo when an email interaction occurs, including delivery status changes, opens, clicks, bounces, and spam reports.
layout: schema
name: Brevo Email Event
properties_list:
- description: Type of email event that occurred.
  name: event
  type: string
- description: Recipient email address associated with the event.
  name: email
  type: string
- description: Internal Brevo event identifier.
  name: id
  type: integer
- description: UTC date-time when the event occurred.
  name: date
  type: string
- description: Unique identifier of the email message that triggered the event.
  name: messageId
  type: string
- description: Subject line of the email message.
  name: subject
  type: string
- description: Tag assigned to the email for categorization and tracking.
  name: tag
  type: string
- description: IP address of the server used to send the email.
  name: sendingIp
  type: string
- description: Unix timestamp in seconds when the event occurred.
  name: ts
  type: integer
- description: Unix timestamp in milliseconds when the event occurred.
  name: ts_epoch
  type: integer
- description: Reason for the event if applicable, such as bounce error codes or spam filter details.
  name: reason
  type: string
- description: URL of the link that was clicked, present only for click events.
  name: link
  type: string
- description: ID of the template used for the email if applicable.
  name: templateId
  type: integer
- description: ID of the marketing campaign if the event is for a campaign email.
  name: campaignId
  type: integer
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-email-event-schema.json
slug: brevo-email-event
tags: []
title: Brevo Email Event
---
