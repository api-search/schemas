---
description: A Zendesk user representing an end user, agent, or admin in the Zendesk Support account. Users are the people who interact with the support system, whether they are customers submitting tickets, agents handling requests, or administrators managing the account. Each user has a role, identity information, and can belong to one or more organizations.
layout: schema
name: Zendesk User
properties_list:
- description: Automatically assigned unique identifier for the user.
  name: id
  type: integer
- description: The API URL of the user resource.
  name: url
  type: string
- description: The full name of the user.
  name: name
  type: string
- description: The primary email address of the user.
  name: email
  type:
  - string
  - 'null'
- description: The primary phone number of the user.
  name: phone
  type:
  - string
  - 'null'
- description: The user's profile photo attachment.
  name: photo
  type:
  - object
  - 'null'
- description: The locale ID for the user, determining their language preferences.
  name: locale_id
  type:
  - integer
  - 'null'
- description: The locale string of the user (e.g., en-US).
  name: locale
  type: string
- description: The IANA time zone of the user (e.g., America/New_York).
  name: time_zone
  type:
  - string
  - 'null'
- description: The ID of the user's default organization.
  name: organization_id
  type:
  - integer
  - 'null'
- description: The role of the user in the Zendesk account.
  name: role
  type: string
- description: The ID of the custom role for agents with non-default permissions.
  name: custom_role_id
  type:
  - integer
  - 'null'
- description: Whether the user's primary identity (email or phone) has been verified.
  name: verified
  type: boolean
- description: An ID from an external system for cross-referencing users.
  name: external_id
  type:
  - string
  - 'null'
- description: Tags applied to the user for segmentation and business rules.
  name: tags
  type: array
- description: An alias displayed to end users instead of the agent's real name.
  name: alias
  type:
  - string
  - 'null'
- description: Whether the user account is currently active.
  name: active
  type: boolean
- description: Whether the user is shared from a different Zendesk Support instance.
  name: shared
  type: boolean
- description: Whether the user is a shared agent from a different Zendesk Support instance.
  name: shared_agent
  type: boolean
- description: Whether the user's phone number is shared with another user.
  name: shared_phone_number
  type:
  - boolean
  - 'null'
- description: The agent's signature text, appended to their comments.
  name: signature
  type:
  - string
  - 'null'
- description: Details about the user, visible only to agents.
  name: details
  type:
  - string
  - 'null'
- description: Internal notes about the user, visible only to agents.
  name: notes
  type:
  - string
  - 'null'
- description: Whether the agent has role-based restrictions.
  name: restricted_agent
  type: boolean
- description: Whether the user account is suspended. Suspended users cannot sign in and their tickets are suspended.
  name: suspended
  type: boolean
- description: The default group ID for the agent.
  name: default_group_id
  type:
  - integer
  - 'null'
- description: Whether the user has permission to access CSV reports.
  name: report_csv
  type: boolean
- description: Whether the user can only create private (internal) comments.
  name: only_private_comments
  type: boolean
- description: The scope of tickets the agent can access.
  name: ticket_restriction
  type:
  - string
  - 'null'
- description: Whether the user has moderator privileges in the community forums.
  name: moderator
  type: boolean
- description: Whether the agent is limited to chat-only access.
  name: chat_only
  type: boolean
- description: Whether two-factor authentication is enabled for the user.
  name: two_factor_auth_enabled
  type:
  - boolean
  - 'null'
- description: Custom user field values as key-value pairs. Keys are the field keys defined via the User Fields API.
  name: user_fields
  type: object
- description: The last time the user signed in, in ISO 8601 format.
  name: last_login_at
  type:
  - string
  - 'null'
- description: When the user was created, in ISO 8601 format.
  name: created_at
  type: string
- description: When the user was last updated, in ISO 8601 format.
  name: updated_at
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-user-schema.json
slug: zendesk-user
source_filename: zendesk-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-user-schema.json\",\n  \"title\": \"Zendesk User\",\n  \"description\": \"A Zendesk user representing an end user, agent, or admin in the Zendesk Support account. Users are the people who interact with the support system, whether they are customers submitting tickets, agents handling requests, or administrators managing the account. Each user has a role, identity information, and can belong to one or more organizations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Automatically assigned unique identifier for the user.\",\n      \"readOnly\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL of the user resource.\",\n      \"readOnly\"\
  : true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the user.\"\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The primary email address of the user.\"\n    },\n    \"phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The primary phone number of the user.\"\n    },\n    \"photo\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The user's profile photo attachment.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"file_name\": {\n          \"type\": \"string\"\n        },\n        \"content_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"content_type\": {\n          \"type\": \"string\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n\
  \          \"description\": \"File size in bytes.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              },\n              \"file_name\": {\n                \"type\": \"string\"\n              },\n              \"content_url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\n              },\n              \"content_type\": {\n                \"type\": \"string\"\n              },\n              \"size\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"locale_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The locale ID for the user, determining their language preferences.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The locale string of the user (e.g., en-US).\",\n      \"readOnly\": true\n    },\n    \"time_zone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The IANA time zone of the user (e.g., America/New_York).\"\n    },\n    \"organization_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the user's default organization.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"end-user\", \"agent\", \"admin\"],\n      \"description\": \"The role of the user in the Zendesk account.\"\n    },\n    \"custom_role_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the custom role for agents with non-default permissions.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's primary identity (email or phone) has been verified.\"\n    },\n    \"external_id\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An ID from an external system for cross-referencing users.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags applied to the user for segmentation and business rules.\"\n    },\n    \"alias\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An alias displayed to end users instead of the agent's real name.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is currently active.\",\n      \"readOnly\": true\n    },\n    \"shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is shared from a different Zendesk Support instance.\",\n      \"readOnly\": true\n    },\n    \"shared_agent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a shared agent from a different Zendesk Support instance.\"\
  ,\n      \"readOnly\": true\n    },\n    \"shared_phone_number\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the user's phone number is shared with another user.\",\n      \"readOnly\": true\n    },\n    \"signature\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The agent's signature text, appended to their comments.\"\n    },\n    \"details\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Details about the user, visible only to agents.\"\n    },\n    \"notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Internal notes about the user, visible only to agents.\"\n    },\n    \"restricted_agent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent has role-based restrictions.\",\n      \"readOnly\": true\n    },\n    \"suspended\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is suspended. Suspended users cannot sign in\
  \ and their tickets are suspended.\"\n    },\n    \"default_group_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The default group ID for the agent.\"\n    },\n    \"report_csv\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has permission to access CSV reports.\",\n      \"readOnly\": true\n    },\n    \"only_private_comments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can only create private (internal) comments.\"\n    },\n    \"ticket_restriction\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"organization\", \"groups\", \"assigned\", \"requested\", null],\n      \"description\": \"The scope of tickets the agent can access.\"\n    },\n    \"moderator\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has moderator privileges in the community forums.\"\n    },\n    \"chat_only\": {\n      \"type\": \"boolean\",\n     \
  \ \"description\": \"Whether the agent is limited to chat-only access.\",\n      \"readOnly\": true\n    },\n    \"two_factor_auth_enabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether two-factor authentication is enabled for the user.\",\n      \"readOnly\": true\n    },\n    \"user_fields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom user field values as key-value pairs. Keys are the field keys defined via the User Fields API.\"\n    },\n    \"last_login_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The last time the user signed in, in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user was created, in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the user was last updated, in ISO 8601 format.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"id\", \"name\", \"role\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-user-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: Zendesk User
---
