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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/meeting.json\",\n  \"title\": \"Cisco Webex Meeting\",\n  \"description\": \"Represents a Webex meeting including meeting series, scheduled meetings, and meeting instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the meeting.\"\n    },\n    \"meetingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting number used to join the meeting.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the meeting.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password required to join the meeting.\"\n    },\n    \"meetingType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of meeting.\",\n      \"enum\": [\"meetingSeries\", \"scheduledMeeting\", \"meeting\"]\n\
  \    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the meeting.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for the meeting in IANA format.\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the meeting in ISO 8601 format.\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the meeting in ISO 8601 format.\"\n    },\n    \"hostUserId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the meeting host.\"\n    },\n    \"hostDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the meeting host.\"\n    },\n    \"hostEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the meeting host.\"\n    },\n    \"webLink\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Link to join the meeting from a web browser.\"\n    },\n    \"sipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"SIP address for joining via video system.\"\n    },\n    \"dialInIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address for dial-in access.\"\n    },\n    \"scheduledType\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled type of the meeting.\",\n      \"enum\": [\"meeting\", \"webinar\", \"personalRoomMeeting\"]\n    },\n    \"recurrence\": {\n      \"type\": \"string\",\n      \"description\": \"Recurrence rule in iCalendar format for recurring meetings.\"\n    },\n    \"telephony\": {\n      \"type\": \"object\",\n      \"description\": \"Telephony information for the meeting.\",\n      \"properties\": {\n        \"accessCode\": {\n          \"type\": \"string\",\n          \"description\": \"Access code for telephony.\"\n   \
  \     },\n        \"callInNumbers\": {\n          \"type\": \"array\",\n          \"description\": \"List of call-in numbers.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\"\n              },\n              \"callInNumber\": {\n                \"type\": \"string\"\n              },\n              \"tollType\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"registrationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether registration is enabled for the meeting.\"\n    }\n  },\n  \"required\": [\"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-meeting-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Meeting
---
