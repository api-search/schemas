---
description: Represents a Webex meeting including meeting series, scheduled meetings, and meeting instances.
layout: schema
name: Cisco Webex Meeting
properties_list:
- description: Unique identifier for the meeting.
  name: id
  type: string
- description: Meeting number used to join the meeting.
  name: meetingNumber
  type: string
- description: Title of the meeting.
  name: title
  type: string
- description: Password required to join the meeting.
  name: password
  type: string
- description: Type of meeting.
  name: meetingType
  type: string
- description: Current state of the meeting.
  name: state
  type: string
- description: Time zone for the meeting in IANA format.
  name: timezone
  type: string
- description: Start time of the meeting in ISO 8601 format.
  name: start
  type: string
- description: End time of the meeting in ISO 8601 format.
  name: end
  type: string
- description: Unique identifier for the meeting host.
  name: hostUserId
  type: string
- description: Display name of the meeting host.
  name: hostDisplayName
  type: string
- description: Email address of the meeting host.
  name: hostEmail
  type: string
- description: Link to join the meeting from a web browser.
  name: webLink
  type: string
- description: SIP address for joining via video system.
  name: sipAddress
  type: string
- description: IP address for dial-in access.
  name: dialInIpAddress
  type: string
- description: Scheduled type of the meeting.
  name: scheduledType
  type: string
- description: Recurrence rule in iCalendar format for recurring meetings.
  name: recurrence
  type: string
- description: Telephony information for the meeting.
  name: telephony
  type: object
- description: Whether registration is enabled for the meeting.
  name: registrationEnabled
  type: boolean
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-meeting-schema.json
slug: cisco-webex-meeting
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Meeting
---
