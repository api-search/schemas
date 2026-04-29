---
description: Meeting settings and options.
layout: schema
name: MeetingSettings
properties_list:
- description: Start video when the host joins the meeting.
  name: host_video
  type: boolean
- description: Start video when participants join the meeting.
  name: participant_video
  type: boolean
- description: Host meeting in China.
  name: cn_meeting
  type: boolean
- description: Host meeting in India.
  name: in_meeting
  type: boolean
- description: Allow participants to join before the host.
  name: join_before_host
  type: boolean
- description: Minutes before the host joins that participants can join. 0 - any time, 5 - 5 minutes, 10 - 10 minutes.
  name: jbh_time
  type: integer
- description: Mute participants upon entry.
  name: mute_upon_entry
  type: boolean
- description: Add watermark when viewing a shared screen.
  name: watermark
  type: boolean
- description: Use Personal Meeting ID instead of generated meeting ID.
  name: use_pmi
  type: boolean
- description: Registration approval type. 0 - Automatically approve, 1 - Manually approve, 2 - No registration required.
  name: approval_type
  type: integer
- description: Registration type for recurring meetings. 1 - Register once and attend any, 2 - Register for each, 3 - Register once and choose occurrences.
  name: registration_type
  type: integer
- description: Determine how participants can join the meeting audio.
  name: audio
  type: string
- description: Automatic recording configuration.
  name: auto_recording
  type: string
- description: Only authenticated users can join the meeting.
  name: enforce_login
  type: boolean
- description: Only users with specific email domain(s) can join. Comma separated for multiple domains.
  name: enforce_login_domains
  type: string
- description: Alternative host email addresses. Comma separated for multiple alternative hosts.
  name: alternative_hosts
  type: string
- description: Send email notification to alternative hosts.
  name: alternative_hosts_email_notification
  type: boolean
- description: Close registration after event date.
  name: close_registration
  type: boolean
- description: Enable the waiting room.
  name: waiting_room
  type: boolean
- description: List of countries for global dial-in numbers.
  name: global_dial_in_countries
  type: array
- description: Contact name for meeting registration.
  name: contact_name
  type: string
- description: Contact email for meeting registration.
  name: contact_email
  type: string
- description: Send email notifications to registrants.
  name: registrants_email_notification
  type: boolean
- description: Send confirmation email to registrants.
  name: registrants_confirmation_email
  type: boolean
- description: Require authentication to join.
  name: meeting_authentication
  type: boolean
- description: Meeting authentication option ID.
  name: authentication_option
  type: string
- description: Allowed authentication domains.
  name: authentication_domains
  type: string
- description: Authentication name set in the authentication profile.
  name: authentication_name
  type: string
- description: Show social share buttons on the registration page.
  name: show_share_button
  type: boolean
- description: Allow attendees to join from multiple devices.
  name: allow_multiple_devices
  type: boolean
- description: Meeting encryption type.
  name: encryption_type
  type: string
- description: Approve or block users from specific countries.
  name: approved_or_denied_countries_or_regions
  type: object
- description: Breakout room settings.
  name: breakout_room
  type: object
- description: Language interpretation settings.
  name: language_interpretation
  type: object
- description: Enable focus mode.
  name: focus_mode
  type: boolean
- description: List of users invited to the meeting.
  name: meeting_invitees
  type: array
- description: Make the meeting private.
  name: private_meeting
  type: boolean
- description: Send email notification when meeting starts.
  name: email_notification
  type: boolean
- description: Allow host to save the order of gallery view.
  name: host_save_video_order
  type: boolean
- description: Continuous meeting chat settings.
  name: continuous_meeting_chat
  type: object
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-settings-schema.json
slug: zoom-meeting-meeting-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingSettings\",\n  \"type\": \"object\",\n  \"description\": \"Meeting settings and options.\",\n  \"properties\": {\n    \"host_video\": {\n      \"type\": \"boolean\",\n      \"description\": \"Start video when the host joins the meeting.\"\n    },\n    \"participant_video\": {\n      \"type\": \"boolean\",\n      \"description\": \"Start video when participants join the meeting.\"\n    },\n    \"cn_meeting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Host meeting in China.\"\n    },\n    \"in_meeting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Host meeting in India.\"\n    },\n    \"join_before_host\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow participants to join before the host.\"\n    },\n    \"jbh_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Minutes before the host joins that participants can join. 0 - any\
  \ time, 5 - 5 minutes, 10 - 10 minutes.\"\n    },\n    \"mute_upon_entry\": {\n      \"type\": \"boolean\",\n      \"description\": \"Mute participants upon entry.\"\n    },\n    \"watermark\": {\n      \"type\": \"boolean\",\n      \"description\": \"Add watermark when viewing a shared screen.\"\n    },\n    \"use_pmi\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use Personal Meeting ID instead of generated meeting ID.\"\n    },\n    \"approval_type\": {\n      \"type\": \"integer\",\n      \"description\": \"Registration approval type. 0 - Automatically approve, 1 - Manually approve, 2 - No registration required.\"\n    },\n    \"registration_type\": {\n      \"type\": \"integer\",\n      \"description\": \"Registration type for recurring meetings. 1 - Register once and attend any, 2 - Register for each, 3 - Register once and choose occurrences.\"\n    },\n    \"audio\": {\n      \"type\": \"string\",\n      \"description\": \"Determine how participants can join the meeting\
  \ audio.\"\n    },\n    \"auto_recording\": {\n      \"type\": \"string\",\n      \"description\": \"Automatic recording configuration.\"\n    },\n    \"enforce_login\": {\n      \"type\": \"boolean\",\n      \"description\": \"Only authenticated users can join the meeting.\"\n    },\n    \"enforce_login_domains\": {\n      \"type\": \"string\",\n      \"description\": \"Only users with specific email domain(s) can join. Comma separated for multiple domains.\"\n    },\n    \"alternative_hosts\": {\n      \"type\": \"string\",\n      \"description\": \"Alternative host email addresses. Comma separated for multiple alternative hosts.\"\n    },\n    \"alternative_hosts_email_notification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Send email notification to alternative hosts.\"\n    },\n    \"close_registration\": {\n      \"type\": \"boolean\",\n      \"description\": \"Close registration after event date.\"\n    },\n    \"waiting_room\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Enable the waiting room.\"\n    },\n    \"global_dial_in_countries\": {\n      \"type\": \"array\",\n      \"description\": \"List of countries for global dial-in numbers.\"\n    },\n    \"contact_name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact name for meeting registration.\"\n    },\n    \"contact_email\": {\n      \"type\": \"string\",\n      \"description\": \"Contact email for meeting registration.\"\n    },\n    \"registrants_email_notification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Send email notifications to registrants.\"\n    },\n    \"registrants_confirmation_email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Send confirmation email to registrants.\"\n    },\n    \"meeting_authentication\": {\n      \"type\": \"boolean\",\n      \"description\": \"Require authentication to join.\"\n    },\n    \"authentication_option\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting authentication\
  \ option ID.\"\n    },\n    \"authentication_domains\": {\n      \"type\": \"string\",\n      \"description\": \"Allowed authentication domains.\"\n    },\n    \"authentication_name\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication name set in the authentication profile.\"\n    },\n    \"show_share_button\": {\n      \"type\": \"boolean\",\n      \"description\": \"Show social share buttons on the registration page.\"\n    },\n    \"allow_multiple_devices\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow attendees to join from multiple devices.\"\n    },\n    \"encryption_type\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting encryption type.\"\n    },\n    \"approved_or_denied_countries_or_regions\": {\n      \"type\": \"object\",\n      \"description\": \"Approve or block users from specific countries.\"\n    },\n    \"breakout_room\": {\n      \"type\": \"object\",\n      \"description\": \"Breakout room settings.\"\n    },\n\
  \    \"language_interpretation\": {\n      \"type\": \"object\",\n      \"description\": \"Language interpretation settings.\"\n    },\n    \"focus_mode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable focus mode.\"\n    },\n    \"meeting_invitees\": {\n      \"type\": \"array\",\n      \"description\": \"List of users invited to the meeting.\"\n    },\n    \"private_meeting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Make the meeting private.\"\n    },\n    \"email_notification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Send email notification when meeting starts.\"\n    },\n    \"host_save_video_order\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow host to save the order of gallery view.\"\n    },\n    \"continuous_meeting_chat\": {\n      \"type\": \"object\",\n      \"description\": \"Continuous meeting chat settings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-settings-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingSettings
---
