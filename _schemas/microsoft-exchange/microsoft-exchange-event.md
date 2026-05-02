---
description: Represents a calendar event in a user calendar or the default calendar of a Microsoft 365 group as exposed through the Microsoft Graph Calendar API. Supports single-instance events, recurring events, meetings with attendees, and online meetings.
layout: schema
name: Microsoft Exchange Calendar Event
properties_list:
- description: Unique identifier for the event
  name: id
  type: string
- description: The text of the event's subject line
  name: subject
  type: string
- description: The body of the message associated with the event
  name: body
  type: object
- description: The preview of the event body in text format
  name: bodyPreview
  type: string
- description: The start date, time, and time zone of the event
  name: start
  type: object
- description: The end date, time, and time zone of the event
  name: end
  type: object
- description: The location of the event
  name: location
  type: object
- description: The locations where the event is held or attended from
  name: locations
  type: array
- description: The collection of attendees for the event
  name: attendees
  type: array
- description: The organizer of the event
  name: organizer
  type: object
- description: Whether the event lasts all day
  name: isAllDay
  type: boolean
- description: Whether the event has been canceled
  name: isCancelled
  type: boolean
- description: Whether updates have been sent to attendees
  name: isDraft
  type: boolean
- description: Whether this event has online meeting information
  name: isOnlineMeeting
  type: boolean
- description: Whether the calendar owner is the organizer
  name: isOrganizer
  type: boolean
- description: Whether a reminder alert is set
  name: isReminderOn
  type: boolean
- description: Details for joining the meeting online
  name: onlineMeeting
  type: object
- description: The online meeting service provider
  name: onlineMeetingProvider
  type: string
- description: URL for an online meeting
  name: onlineMeetingUrl
  type: string
- description: The recurrence pattern for the event
  name: recurrence
  type: object
- description: Minutes before start that the reminder alert occurs
  name: reminderMinutesBeforeStart
  type: integer
- description: Whether the organizer requests a response from invitees
  name: responseRequested
  type: boolean
- description: The response status of the event
  name: responseStatus
  type: object
- description: The event sensitivity level
  name: sensitivity
  type: string
- description: ID for the recurring series master
  name: seriesMasterId
  type: string
- description: The status to show during the event
  name: showAs
  type: string
- description: The event type
  name: type
  type: string
- description: The importance of the event
  name: importance
  type: string
- description: Whether the event has attachments
  name: hasAttachments
  type: boolean
- description: The categories associated with the event
  name: categories
  type: array
- description: Whether the organizer allows invitees to propose new times
  name: allowNewTimeProposals
  type: boolean
- description: A unique identifier for the event across calendars
  name: iCalUId
  type: string
- description: Identifies the version of the event
  name: changeKey
  type: string
- description: When the event was created
  name: createdDateTime
  type: string
- description: When the event was last changed
  name: lastModifiedDateTime
  type: string
- description: URL to open the event in Outlook on the web
  name: webLink
  type: string
- description: Custom identifier to avoid duplicate event creation on retries
  name: transactionId
  type: string
- description: When true, each attendee only sees themselves in the meeting request
  name: hideAttendees
  type: boolean
- description: The start time zone set when the event was created
  name: originalStartTimeZone
  type: string
- description: The end time zone set when the event was created
  name: originalEndTimeZone
  type: string
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-event-schema.json
slug: microsoft-exchange-event
source_filename: microsoft-exchange-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-event-schema.json\",\n  \"title\": \"Microsoft Exchange Calendar Event\",\n  \"description\": \"Represents a calendar event in a user calendar or the default calendar of a Microsoft 365 group as exposed through the Microsoft Graph Calendar API. Supports single-instance events, recurring events, meetings with attendees, and online meetings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event\",\n      \"readOnly\": true\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The text of the event's subject line\"\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/itemBody\",\n      \"description\": \"The body of the message associated with the event\"\n    },\n    \"bodyPreview\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The preview of the event body in text format\",\n      \"readOnly\": true\n    },\n    \"start\": {\n      \"$ref\": \"#/$defs/dateTimeTimeZone\",\n      \"description\": \"The start date, time, and time zone of the event\"\n    },\n    \"end\": {\n      \"$ref\": \"#/$defs/dateTimeTimeZone\",\n      \"description\": \"The end date, time, and time zone of the event\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/location\",\n      \"description\": \"The location of the event\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/location\"\n      },\n      \"description\": \"The locations where the event is held or attended from\"\n    },\n    \"attendees\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/attendee\"\n      },\n      \"description\": \"The collection of attendees for the event\"\n    },\n    \"organizer\": {\n      \"$ref\"\
  : \"#/$defs/recipient\",\n      \"description\": \"The organizer of the event\"\n    },\n    \"isAllDay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event lasts all day\"\n    },\n    \"isCancelled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event has been canceled\",\n      \"readOnly\": true\n    },\n    \"isDraft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether updates have been sent to attendees\",\n      \"readOnly\": true\n    },\n    \"isOnlineMeeting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this event has online meeting information\"\n    },\n    \"isOrganizer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the calendar owner is the organizer\",\n      \"readOnly\": true\n    },\n    \"isReminderOn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a reminder alert is set\"\n    },\n    \"onlineMeeting\": {\n      \"$ref\": \"#/$defs/onlineMeetingInfo\"\
  ,\n      \"description\": \"Details for joining the meeting online\"\n    },\n    \"onlineMeetingProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"teamsForBusiness\", \"skypeForBusiness\", \"skypeForConsumer\"],\n      \"description\": \"The online meeting service provider\"\n    },\n    \"onlineMeetingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for an online meeting\",\n      \"readOnly\": true\n    },\n    \"recurrence\": {\n      \"$ref\": \"#/$defs/patternedRecurrence\",\n      \"description\": \"The recurrence pattern for the event\"\n    },\n    \"reminderMinutesBeforeStart\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Minutes before start that the reminder alert occurs\"\n    },\n    \"responseRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organizer requests a response from invitees\"\n    },\n    \"responseStatus\": {\n      \"\
  $ref\": \"#/$defs/responseStatus\",\n      \"description\": \"The response status of the event\"\n    },\n    \"sensitivity\": {\n      \"type\": \"string\",\n      \"enum\": [\"normal\", \"personal\", \"private\", \"confidential\"],\n      \"description\": \"The event sensitivity level\"\n    },\n    \"seriesMasterId\": {\n      \"type\": \"string\",\n      \"description\": \"ID for the recurring series master\",\n      \"readOnly\": true\n    },\n    \"showAs\": {\n      \"type\": \"string\",\n      \"enum\": [\"free\", \"tentative\", \"busy\", \"oof\", \"workingElsewhere\", \"unknown\"],\n      \"description\": \"The status to show during the event\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"singleInstance\", \"occurrence\", \"exception\", \"seriesMaster\"],\n      \"description\": \"The event type\",\n      \"readOnly\": true\n    },\n    \"importance\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"normal\", \"high\"],\n      \"description\"\
  : \"The importance of the event\"\n    },\n    \"hasAttachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event has attachments\",\n      \"readOnly\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The categories associated with the event\"\n    },\n    \"allowNewTimeProposals\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organizer allows invitees to propose new times\"\n    },\n    \"iCalUId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the event across calendars\",\n      \"readOnly\": true\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the version of the event\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event was created\"\
  ,\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event was last changed\",\n      \"readOnly\": true\n    },\n    \"webLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to open the event in Outlook on the web\",\n      \"readOnly\": true\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Custom identifier to avoid duplicate event creation on retries\"\n    },\n    \"hideAttendees\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, each attendee only sees themselves in the meeting request\"\n    },\n    \"originalStartTimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The start time zone set when the event was created\"\n    },\n    \"originalEndTimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The end time zone set when the event\
  \ was created\"\n    }\n  },\n  \"required\": [\"subject\", \"start\", \"end\"],\n  \"$defs\": {\n    \"attendee\": {\n      \"type\": \"object\",\n      \"description\": \"An event attendee with response status\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"$ref\": \"#/$defs/emailAddress\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"required\", \"optional\", \"resource\"],\n          \"description\": \"The type of attendee\"\n        },\n        \"status\": {\n          \"$ref\": \"#/$defs/responseStatus\"\n        }\n      }\n    },\n    \"recipient\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"$ref\": \"#/$defs/emailAddress\"\n        }\n      }\n    },\n    \"emailAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name\"\n        },\n        \"address\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address\"\n        }\n      }\n    },\n    \"itemBody\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contentType\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"html\"]\n        },\n        \"content\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"dateTimeTimeZone\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a date, time, and time zone\",\n      \"properties\": {\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"description\": \"A date and time in ISO 8601 format\"\n        },\n        \"timeZone\": {\n          \"type\": \"string\",\n          \"description\": \"A time zone name\"\n        }\n      },\n      \"required\": [\"dateTime\", \"timeZone\"]\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Represents location information\"\
  ,\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the location\"\n        },\n        \"locationType\": {\n          \"type\": \"string\",\n          \"enum\": [\"default\", \"conferenceRoom\", \"homeAddress\", \"businessAddress\", \"geoCoordinates\", \"streetAddress\", \"hotel\", \"restaurant\", \"localBusiness\", \"postalAddress\"]\n        },\n        \"locationUri\": {\n          \"type\": \"string\"\n        },\n        \"locationEmailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/physicalAddress\"\n        },\n        \"coordinates\": {\n          \"$ref\": \"#/$defs/geoCoordinates\"\n        }\n      }\n    },\n    \"physicalAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": {\
  \ \"type\": \"string\" },\n        \"countryOrRegion\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" }\n      }\n    },\n    \"geoCoordinates\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"latitude\": { \"type\": \"number\" },\n        \"longitude\": { \"type\": \"number\" },\n        \"accuracy\": { \"type\": \"number\" },\n        \"altitude\": { \"type\": \"number\" },\n        \"altitudeAccuracy\": { \"type\": \"number\" }\n      }\n    },\n    \"onlineMeetingInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Details for joining an online meeting\",\n      \"properties\": {\n        \"joinUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to join the online meeting\"\n        },\n        \"conferenceId\": {\n          \"type\": \"string\"\n        },\n        \"tollNumber\": {\n          \"type\": \"string\"\n        },\n        \"tollFreeNumbers\": {\n       \
  \   \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"quickDial\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"responseStatus\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"response\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"organizer\", \"tentativelyAccepted\", \"accepted\", \"declined\", \"notResponded\"]\n        },\n        \"time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"patternedRecurrence\": {\n      \"type\": \"object\",\n      \"description\": \"The recurrence pattern and range\",\n      \"properties\": {\n        \"pattern\": {\n          \"$ref\": \"#/$defs/recurrencePattern\"\n        },\n        \"range\": {\n          \"$ref\": \"#/$defs/recurrenceRange\"\n        }\n      }\n    },\n    \"recurrencePattern\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n \
  \         \"type\": \"string\",\n          \"enum\": [\"daily\", \"weekly\", \"absoluteMonthly\", \"relativeMonthly\", \"absoluteYearly\", \"relativeYearly\"]\n        },\n        \"interval\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        },\n        \"month\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 12\n        },\n        \"dayOfMonth\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 31\n        },\n        \"daysOfWeek\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"sunday\", \"monday\", \"tuesday\", \"wednesday\", \"thursday\", \"friday\", \"saturday\"]\n          }\n        },\n        \"firstDayOfWeek\": {\n          \"type\": \"string\",\n          \"enum\": [\"sunday\", \"monday\", \"tuesday\", \"wednesday\", \"thursday\", \"friday\", \"saturday\"]\n        },\n        \"index\": {\n          \"\
  type\": \"string\",\n          \"enum\": [\"first\", \"second\", \"third\", \"fourth\", \"last\"]\n        }\n      }\n    },\n    \"recurrenceRange\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"endDate\", \"noEnd\", \"numbered\"]\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"recurrenceTimeZone\": {\n          \"type\": \"string\"\n        },\n        \"numberOfOccurrences\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-event-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Calendar Event
---
