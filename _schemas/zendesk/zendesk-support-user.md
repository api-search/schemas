---
description: A Zendesk user representing an end user, agent, or admin in the account.
layout: schema
name: User
properties_list:
- description: Automatically assigned user ID.
  name: id
  type: integer
- description: The API URL of the user.
  name: url
  type: string
- description: The name of the user.
  name: name
  type: string
- description: The primary email address of the user.
  name: email
  type: string
- description: The primary phone number of the user.
  name: phone
  type: string
- description: The user's profile photo.
  name: photo
  type: object
- description: The locale ID of the user.
  name: locale_id
  type: integer
- description: The locale of the user (e.g., en-US).
  name: locale
  type: string
- description: The time zone of the user.
  name: time_zone
  type: string
- description: The ID of the user's default organization.
  name: organization_id
  type: integer
- description: The role of the user.
  name: role
  type: string
- description: The custom role ID for agents with custom roles.
  name: custom_role_id
  type: integer
- description: Whether the user's identity has been verified.
  name: verified
  type: boolean
- description: An external ID for the user from an integrated system.
  name: external_id
  type: string
- description: Tags applied to the user.
  name: tags
  type: array
- description: An alias displayed instead of the agent's name.
  name: alias
  type: string
- description: Whether the user account is active.
  name: active
  type: boolean
- description: Whether the user is shared from a different Zendesk Support instance.
  name: shared
  type: boolean
- description: Whether the user is a shared agent from a different instance.
  name: shared_agent
  type: boolean
- description: Whether the phone number is shared.
  name: shared_phone_number
  type: boolean
- description: The signature text appended to the agent's comments.
  name: signature
  type: string
- description: Details about the user visible only to agents.
  name: details
  type: string
- description: Notes about the user visible only to agents.
  name: notes
  type: string
- description: Whether the agent has restrictions (true for agents in a custom role with restrictions).
  name: restricted_agent
  type: boolean
- description: Whether the user is suspended.
  name: suspended
  type: boolean
- description: The default group ID for the agent.
  name: default_group_id
  type: integer
- description: Whether the user can access the CSV report.
  name: report_csv
  type: boolean
- description: Whether the user can only create private comments (for restricted end users).
  name: only_private_comments
  type: boolean
- description: The ticket access restriction for the agent.
  name: ticket_restriction
  type: string
- description: Whether the user has community moderator privileges.
  name: moderator
  type: boolean
- description: Whether the user is a chat-only agent.
  name: chat_only
  type: boolean
- description: Whether two-factor authentication is enabled.
  name: two_factor_auth_enabled
  type: boolean
- description: Custom user field values (key-value pairs).
  name: user_fields
  type: object
- description: The last time the user signed in (ISO 8601).
  name: last_login_at
  type: string
- description: When the user was created (ISO 8601).
  name: created_at
  type: string
- description: When the user was last updated (ISO 8601).
  name: updated_at
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-user-schema.json
slug: zendesk-support-user
source_filename: zendesk-support-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A Zendesk user representing an end user, agent, or admin in the account.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Automatically assigned user ID.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The API URL of the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The primary email address of the user.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The primary phone number of the user.\"\n    },\n    \"photo\": {\n      \"type\": \"object\",\n      \"description\": \"The user's profile photo.\"\n    },\n    \"locale_id\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  The locale ID of the user.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The locale of the user (e.g., en-US).\"\n    },\n    \"time_zone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone of the user.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user's default organization.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the user.\"\n    },\n    \"custom_role_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The custom role ID for agents with custom roles.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's identity has been verified.\"\n    },\n    \"external_id\": {\n      \"type\": \"string\",\n      \"description\": \"An external ID for the user from an integrated system.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Tags applied to the user.\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"An alias displayed instead of the agent's name.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active.\"\n    },\n    \"shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is shared from a different Zendesk Support instance.\"\n    },\n    \"shared_agent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a shared agent from a different instance.\"\n    },\n    \"shared_phone_number\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the phone number is shared.\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"description\": \"The signature text appended to the agent's comments.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Details about the user visible only to agents.\"\n\
  \    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes about the user visible only to agents.\"\n    },\n    \"restricted_agent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent has restrictions (true for agents in a custom role with restrictions).\"\n    },\n    \"suspended\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is suspended.\"\n    },\n    \"default_group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The default group ID for the agent.\"\n    },\n    \"report_csv\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can access the CSV report.\"\n    },\n    \"only_private_comments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can only create private comments (for restricted end users).\"\n    },\n    \"ticket_restriction\": {\n      \"type\": \"string\",\n      \"description\": \"The ticket access restriction for\
  \ the agent.\"\n    },\n    \"moderator\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has community moderator privileges.\"\n    },\n    \"chat_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a chat-only agent.\"\n    },\n    \"two_factor_auth_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether two-factor authentication is enabled.\"\n    },\n    \"user_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom user field values (key-value pairs).\"\n    },\n    \"last_login_at\": {\n      \"type\": \"string\",\n      \"description\": \"The last time the user signed in (ISO 8601).\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the user was created (ISO 8601).\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the user was last updated (ISO 8601).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-user-schema.json
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
title: User
---
