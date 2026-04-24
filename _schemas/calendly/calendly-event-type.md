---
description: An event type defines a kind of meeting that can be scheduled through Calendly, including its name, duration, location configuration, custom questions, and availability settings.
layout: schema
name: Calendly Event Type
properties_list:
- description: The canonical URI of the event type resource.
  name: uri
  type: string
- description: The name of the event type displayed to invitees.
  name: name
  type: string
- description: Whether the event type is currently active and available for scheduling.
  name: active
  type: boolean
- description: The booking method for the event type.
  name: booking_method
  type: string
- description: The URL-friendly slug for the event type.
  name: slug
  type: string
- description: The public URL of the event type's scheduling page.
  name: scheduling_url
  type: string
- description: The default duration of the event in minutes.
  name: duration
  type: integer
- description: Whether the event type is for one-on-one or group meetings.
  name: kind
  type: string
- description: For team event types, the strategy for assigning hosts to meetings.
  name: pooling_type
  type:
  - string
  - 'null'
- description: The type classification of the event type.
  name: type
  type: string
- description: The hex color code associated with the event type for display purposes.
  name: color
  type: string
- description: The plain text description of the event type.
  name: description_plain
  type:
  - string
  - 'null'
- description: The HTML-formatted description of the event type.
  name: description_html
  type:
  - string
  - 'null'
- description: An internal note visible only to the event host, not shown to invitees.
  name: internal_note
  type:
  - string
  - 'null'
- description: ''
  name: profile
  type: object
- description: Whether the event type is hidden from the user's public scheduling page.
  name: secret
  type: boolean
- description: The timestamp when the event type was deleted, if applicable.
  name: deleted_at
  type:
  - string
  - 'null'
- description: Custom questions displayed on the booking page for invitees to answer.
  name: custom_questions
  type: array
- description: The timestamp when the event type was created.
  name: created_at
  type: string
- description: The timestamp when the event type was last updated.
  name: updated_at
  type: string
provider_name: Calendly
provider_slug: calendly
schema_file: json-schema/calendly-event-type-schema.json
slug: calendly-event-type
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Event Type
---
