---
description: An invitee is a person who has booked or been booked for a scheduled event in Calendly, including their contact information, booking details, custom question answers, and tracking parameters.
layout: schema
name: Calendly Invitee
properties_list:
- description: The canonical URI of the invitee resource.
  name: uri
  type: string
- description: The email address of the invitee.
  name: email
  type: string
- description: The first name of the invitee.
  name: first_name
  type: string
- description: The last name of the invitee.
  name: last_name
  type: string
- description: The full name of the invitee.
  name: name
  type: string
- description: The current status of the invitee.
  name: status
  type: string
- description: The IANA timezone of the invitee (e.g., America/New_York).
  name: timezone
  type: string
- description: The URI of the associated scheduled event.
  name: event
  type: string
- description: The phone number for text reminders, if provided.
  name: text_reminder_number
  type:
  - string
  - 'null'
- description: Whether this invitee was rescheduled from a previous event.
  name: rescheduled
  type: boolean
- description: The URI of the previous invitee if this was a rescheduled booking.
  name: old_invitee
  type:
  - string
  - 'null'
- description: The URI of the new invitee if this booking was rescheduled to a new one.
  name: new_invitee
  type:
  - string
  - 'null'
- description: The URL for the invitee to cancel the event.
  name: cancel_url
  type: string
- description: The URL for the invitee to reschedule the event.
  name: reschedule_url
  type: string
- description: The URI of the routing form submission that led to this booking, if applicable.
  name: routing_form_submission
  type:
  - string
  - 'null'
- description: ''
  name: cancellation
  type: object
- description: ''
  name: payment
  type: object
- description: The invitee's answers to custom questions on the event type booking page.
  name: questions_and_answers
  type: array
- description: ''
  name: tracking
  type: object
- description: The timestamp when the invitee was created.
  name: created_at
  type: string
- description: The timestamp when the invitee was last updated.
  name: updated_at
  type: string
provider_name: Calendly
provider_slug: calendly
schema_file: json-schema/calendly-invitee-schema.json
slug: calendly-invitee
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Invitee
---
