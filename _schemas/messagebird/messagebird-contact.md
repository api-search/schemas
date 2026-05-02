---
description: Represents a contact in the MessageBird address book that can be associated with multiple communication channels.
layout: schema
name: MessageBird Contact
properties_list:
- description: The unique identifier of the contact.
  name: id
  type: string
- description: The URL of the contact resource.
  name: href
  type: string
- description: The phone number of the contact in international format.
  name: msisdn
  type: string
- description: The first name of the contact.
  name: firstName
  type: string
- description: The last name of the contact.
  name: lastName
  type: string
- description: Custom field 1 for arbitrary contact data.
  name: custom1
  type: string
- description: Custom field 2 for arbitrary contact data.
  name: custom2
  type: string
- description: Custom field 3 for arbitrary contact data.
  name: custom3
  type: string
- description: Custom field 4 for arbitrary contact data.
  name: custom4
  type: string
- description: Links to the groups the contact belongs to.
  name: groups
  type: object
- description: Links to messages associated with the contact.
  name: messages
  type: object
- description: The date and time when the contact was created.
  name: createdDatetime
  type: string
- description: The date and time when the contact was last updated.
  name: updatedDatetime
  type: string
provider_name: messagebird
provider_slug: messagebird
schema_file: json-schema/messagebird-contact-schema.json
slug: messagebird-contact
source_filename: messagebird-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/messagebird/contact.json\",\n  \"title\": \"MessageBird Contact\",\n  \"description\": \"Represents a contact in the MessageBird address book that can be associated with multiple communication channels.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"msisdn\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the contact.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the contact resource.\"\n    },\n    \"msisdn\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the contact in international format.\",\n      \"pattern\": \"^\\\\+?[1-9]\\\\d{1,14}$\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the contact.\",\n      \"maxLength\"\
  : 256\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the contact.\",\n      \"maxLength\": 256\n    },\n    \"custom1\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field 1 for arbitrary contact data.\"\n    },\n    \"custom2\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field 2 for arbitrary contact data.\"\n    },\n    \"custom3\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field 3 for arbitrary contact data.\"\n    },\n    \"custom4\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field 4 for arbitrary contact data.\"\n    },\n    \"groups\": {\n      \"type\": \"object\",\n      \"description\": \"Links to the groups the contact belongs to.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to retrieve the groups.\"\n        },\n        \"totalCount\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"The total number of groups.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"messages\": {\n      \"type\": \"object\",\n      \"description\": \"Links to messages associated with the contact.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to retrieve messages.\"\n        },\n        \"totalCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of messages.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"createdDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the contact was created.\"\n    },\n    \"updatedDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the contact was last updated.\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/json-schema/messagebird-contact-schema.json
tags: []
title: MessageBird Contact
---
