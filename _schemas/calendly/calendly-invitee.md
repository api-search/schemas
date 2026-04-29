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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.calendly.com/schemas/calendly/invitee.json\",\n  \"title\": \"Calendly Invitee\",\n  \"description\": \"An invitee is a person who has booked or been booked for a scheduled event in Calendly, including their contact information, booking details, custom question answers, and tracking parameters.\",\n  \"type\": \"object\",\n  \"required\": [\"uri\", \"email\", \"name\", \"status\", \"event\"],\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The canonical URI of the invitee resource.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the invitee.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the invitee.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The last name of the invitee.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the invitee.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"canceled\"],\n      \"description\": \"The current status of the invitee.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The IANA timezone of the invitee (e.g., America/New_York).\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI of the associated scheduled event.\"\n    },\n    \"text_reminder_number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The phone number for text reminders, if provided.\"\n    },\n    \"rescheduled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this invitee was rescheduled from a previous event.\"\n    },\n    \"old_invitee\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URI of the previous invitee if this was a rescheduled booking.\"\n    },\n    \"new_invitee\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URI of the new invitee if this booking was rescheduled to a new one.\"\n    },\n    \"cancel_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for the invitee to cancel the event.\"\n    },\n    \"reschedule_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for the invitee to reschedule the event.\"\n    },\n    \"routing_form_submission\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URI of the routing form submission that led to this booking, if applicable.\"\n    },\n    \"cancellation\": {\n      \"$ref\": \"#/$defs/Cancellation\"\n    },\n    \"payment\": {\n      \"\
  $ref\": \"#/$defs/Payment\"\n    },\n    \"questions_and_answers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/QuestionAndAnswer\"\n      },\n      \"description\": \"The invitee's answers to custom questions on the event type booking page.\"\n    },\n    \"tracking\": {\n      \"$ref\": \"#/$defs/Tracking\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the invitee was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the invitee was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Cancellation\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the cancellation of the invitee's booking.\",\n      \"properties\": {\n        \"canceled_by\": {\n          \"type\": \"string\",\n          \"description\": \"The name or identifier of the\
  \ person who canceled.\"\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"maxLength\": 10000,\n          \"description\": \"The reason provided for the cancellation.\"\n        },\n        \"canceler_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"host\", \"invitee\"],\n          \"description\": \"Whether the host or the invitee canceled.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp when the cancellation occurred.\"\n        }\n      }\n    },\n    \"Payment\": {\n      \"type\": \"object\",\n      \"description\": \"Payment information if the event type requires payment.\",\n      \"properties\": {\n        \"external_id\": {\n          \"type\": \"string\",\n          \"description\": \"The external payment processor transaction ID.\"\n        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"enum\"\
  : [\"stripe\", \"paypal\"],\n          \"description\": \"The payment provider used.\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"The payment amount.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"The three-letter ISO 4217 currency code.\"\n        },\n        \"terms\": {\n          \"type\": \"string\",\n          \"description\": \"The payment terms displayed to the invitee.\"\n        },\n        \"successful\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the payment was successfully processed.\"\n        }\n      }\n    },\n    \"QuestionAndAnswer\": {\n      \"type\": \"object\",\n      \"description\": \"A custom question and the invitee's answer from the booking page.\",\n      \"properties\": {\n        \"question\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The text of the custom question.\"\n        },\n        \"answer\": {\n          \"type\": \"string\",\n          \"description\": \"The invitee's answer to the question.\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The display position of the question on the booking page.\"\n        }\n      }\n    },\n    \"Tracking\": {\n      \"type\": \"object\",\n      \"description\": \"UTM and tracking parameters captured at booking time for attribution.\",\n      \"properties\": {\n        \"utm_campaign\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UTM campaign parameter.\"\n        },\n        \"utm_source\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UTM source parameter.\"\n        },\n        \"utm_medium\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UTM medium parameter.\"\n        },\n \
  \       \"utm_content\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UTM content parameter.\"\n        },\n        \"utm_term\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UTM term parameter.\"\n        },\n        \"salesforce_uuid\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The Salesforce UUID for CRM attribution.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/json-schema/calendly-invitee-schema.json
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Invitee
---
