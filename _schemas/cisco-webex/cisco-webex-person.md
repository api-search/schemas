---
description: Represents a user in the Webex platform including profile information, contact details, roles, and licenses.
layout: schema
name: Cisco Webex Person
properties_list:
- description: Unique identifier for the person.
  name: id
  type: string
- description: Email addresses associated with the person.
  name: emails
  type: array
- description: Phone numbers for the person.
  name: phoneNumbers
  type: array
- description: SIP addresses of the person.
  name: sipAddresses
  type: array
- description: Webex Calling extension number.
  name: extension
  type: string
- description: Location ID for Webex Calling.
  name: locationId
  type: string
- description: Full display name of the person.
  name: displayName
  type: string
- description: Nickname of the person.
  name: nickName
  type: string
- description: First name of the person.
  name: firstName
  type: string
- description: Last name of the person.
  name: lastName
  type: string
- description: URL to the person's avatar image.
  name: avatar
  type: string
- description: Organization ID the person belongs to.
  name: orgId
  type: string
- description: Role IDs assigned to the person.
  name: roles
  type: array
- description: License IDs assigned to the person.
  name: licenses
  type: array
- description: Department of the person.
  name: department
  type: string
- description: Manager name of the person.
  name: manager
  type: string
- description: Person ID of the manager.
  name: managerId
  type: string
- description: Job title of the person.
  name: title
  type: string
- description: Physical addresses of the person.
  name: addresses
  type: array
- description: Date and time the person was created.
  name: created
  type: string
- description: Date and time the person was last modified.
  name: lastModified
  type: string
- description: Time zone of the person in IANA format.
  name: timezone
  type: string
- description: Date and time of the person's last activity.
  name: lastActivity
  type: string
- description: Webex site URLs associated with the person.
  name: siteUrls
  type: array
- description: Current presence status of the person.
  name: status
  type: string
- description: Type of the person account.
  name: type
  type: string
- description: Whether the invite is pending acceptance.
  name: invitePending
  type: boolean
- description: Whether the person's login is enabled.
  name: loginEnabled
  type: boolean
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-person-schema.json
slug: cisco-webex-person
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/person.json\",\n  \"title\": \"Cisco Webex Person\",\n  \"description\": \"Represents a user in the Webex platform including profile information, contact details, roles, and licenses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the person.\"\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses associated with the person.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"Phone numbers for the person.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Phone number type (e.g.,\
  \ work, mobile).\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Phone number value.\"\n          }\n        }\n      }\n    },\n    \"sipAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"SIP addresses of the person.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"primary\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"extension\": {\n      \"type\": \"string\",\n      \"description\": \"Webex Calling extension number.\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location ID for Webex Calling.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the person.\"\n    },\n    \"nickName\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Nickname of the person.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the person.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the person.\"\n    },\n    \"avatar\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the person's avatar image.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization ID the person belongs to.\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"description\": \"Role IDs assigned to the person.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"licenses\": {\n      \"type\": \"array\",\n      \"description\": \"License IDs assigned to the person.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"department\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Department of the person.\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"description\": \"Manager name of the person.\"\n    },\n    \"managerId\": {\n      \"type\": \"string\",\n      \"description\": \"Person ID of the manager.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title of the person.\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"Physical addresses of the person.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"streetAddress\": {\n            \"type\": \"string\"\n          },\n          \"locality\": {\n            \"type\": \"string\"\n          },\n          \"region\": {\n            \"type\": \"string\"\n          },\n          \"postalCode\": {\n            \"type\": \"string\"\n          },\n          \"country\": {\n            \"\
  type\": \"string\"\n          }\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the person was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the person was last modified.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone of the person in IANA format.\"\n    },\n    \"lastActivity\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the person's last activity.\"\n    },\n    \"siteUrls\": {\n      \"type\": \"array\",\n      \"description\": \"Webex site URLs associated with the person.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current presence status of the person.\",\n      \"enum\"\
  : [\"active\", \"call\", \"DoNotDisturb\", \"inactive\", \"meeting\", \"OutOfOffice\", \"pending\", \"presenting\", \"unknown\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the person account.\",\n      \"enum\": [\"person\", \"bot\", \"appuser\"]\n    },\n    \"invitePending\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the invite is pending acceptance.\"\n    },\n    \"loginEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person's login is enabled.\"\n    }\n  },\n  \"required\": [\"id\", \"emails\", \"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-person-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Person
---
