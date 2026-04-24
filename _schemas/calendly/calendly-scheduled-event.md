---
description: A scheduled event represents a booked meeting in Calendly with a specific start time, end time, location, host memberships, and associated invitees.
layout: schema
name: Calendly Scheduled Event
properties_list:
- description: The canonical URI of the scheduled event resource.
  name: uri
  type: string
- description: The name of the scheduled event, inherited from the event type.
  name: name
  type: string
- description: The current status of the scheduled event.
  name: status
  type: string
- description: The start time of the event in UTC (ISO 8601 format).
  name: start_time
  type: string
- description: The end time of the event in UTC (ISO 8601 format).
  name: end_time
  type: string
- description: The URI of the event type this event was created from.
  name: event_type
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: invitees_counter
  type: object
- description: ''
  name: cancellation
  type: object
- description: The list of users who are members (hosts) of this event.
  name: event_memberships
  type: array
- description: Additional guests invited to the event beyond the primary invitee.
  name: event_guests
  type: array
- description: The timestamp when the event was created.
  name: created_at
  type: string
- description: The timestamp when the event was last updated.
  name: updated_at
  type: string
provider_name: Calendly
provider_slug: calendly
schema_file: json-schema/calendly-scheduled-event-schema.json
slug: calendly-scheduled-event
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Scheduled Event
---
