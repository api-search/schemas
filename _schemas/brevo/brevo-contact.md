---
description: Represents a contact in the Brevo platform with email, phone, attributes, and list memberships used for transactional and marketing messaging.
layout: schema
name: Brevo Contact
properties_list:
- description: Unique internal identifier of the contact.
  name: id
  type: integer
- description: Primary email address of the contact.
  name: email
  type: string
- description: Phone number of the contact in international format.
  name: phone
  type: string
- description: Whether the contact's email address is blacklisted from receiving messages.
  name: emailBlacklisted
  type: boolean
- description: Whether the contact's phone number is blacklisted from receiving SMS.
  name: smsBlacklisted
  type: boolean
- description: IDs of contact lists the contact belongs to.
  name: listIds
  type: array
- description: Custom attribute values for the contact profile as key-value pairs. Keys correspond to attribute names defined in the account.
  name: attributes
  type: object
- description: UTC date-time when the contact was created.
  name: createdAt
  type: string
- description: UTC date-time when the contact was last modified.
  name: modifiedAt
  type: string
- description: Email campaign interaction statistics for the contact.
  name: statistics
  type: object
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-contact-schema.json
slug: brevo-contact
source_filename: brevo-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://brevo.com/schemas/brevo/contact.json\",\n  \"title\": \"Brevo Contact\",\n  \"description\": \"Represents a contact in the Brevo platform with email, phone, attributes, and list memberships used for transactional and marketing messaging.\",\n  \"type\": \"object\",\n  \"required\": [\"email\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique internal identifier of the contact.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address of the contact.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the contact in international format.\",\n      \"pattern\": \"^\\\\+?[1-9]\\\\d{1,14}$\"\n    },\n    \"emailBlacklisted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact's email address\
  \ is blacklisted from receiving messages.\",\n      \"default\": false\n    },\n    \"smsBlacklisted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact's phone number is blacklisted from receiving SMS.\",\n      \"default\": false\n    },\n    \"listIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of contact lists the contact belongs to.\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom attribute values for the contact profile as key-value pairs. Keys correspond to attribute names defined in the account.\",\n      \"additionalProperties\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC date-time when the contact was created.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC date-time\
  \ when the contact was last modified.\"\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Email campaign interaction statistics for the contact.\",\n      \"properties\": {\n        \"messagesSent\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of emails sent to the contact.\",\n          \"minimum\": 0\n        },\n        \"hardBounces\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of hard bounces for the contact.\",\n          \"minimum\": 0\n        },\n        \"softBounces\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of soft bounces for the contact.\",\n          \"minimum\": 0\n        },\n        \"opened\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of emails opened by the contact.\",\n          \"minimum\": 0\n        },\n        \"clicked\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Total number of email links clicked by the contact.\",\n          \"minimum\": 0\n        },\n        \"unsubscriptions\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of unsubscription actions by the contact.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"ContactAttribute\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a custom contact attribute used to extend contact profiles with additional data fields.\",\n      \"required\": [\"name\", \"category\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the attribute.\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Category grouping for the attribute.\",\n          \"enum\": [\"normal\", \"transactional\", \"category\", \"calculated\", \"global\"]\n   \
  \     },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the attribute value.\",\n          \"enum\": [\"text\", \"date\", \"float\", \"boolean\", \"id\"]\n        },\n        \"enumeration\": {\n          \"type\": \"array\",\n          \"description\": \"Possible enumeration values for category-type attributes.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"value\", \"label\"],\n            \"properties\": {\n              \"value\": {\n                \"type\": \"integer\",\n                \"description\": \"Numeric value of the enum option.\"\n              },\n              \"label\": {\n                \"type\": \"string\",\n                \"description\": \"Display label for the enum option.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ContactList\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a contact list used to organize\
  \ contacts into groups for targeted campaign sending.\",\n      \"required\": [\"name\", \"folderId\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the list.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the contact list.\",\n          \"minLength\": 1\n        },\n        \"totalSubscribers\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of subscribed contacts in the list.\",\n          \"minimum\": 0\n        },\n        \"totalBlacklisted\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of blacklisted contacts in the list.\",\n          \"minimum\": 0\n        },\n        \"folderId\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the folder containing the list.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"UTC date-time when the list was created.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/json-schema/brevo-contact-schema.json
tags: []
title: Brevo Contact
---
