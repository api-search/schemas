---
description: A Zendesk Support ticket representing a customer service request. Tickets are the core entity in Zendesk Support, capturing the communication between a customer and support agents. Each ticket has a lifecycle from creation through resolution, with statuses, priorities, assignees, and a full audit trail of changes and comments.
layout: schema
name: Zendesk Ticket
properties_list:
- description: Automatically assigned unique identifier for the ticket.
  name: id
  type: integer
- description: The API URL of the ticket resource.
  name: url
  type: string
- description: An optional ID from an external system used to link the ticket to records outside Zendesk.
  name: external_id
  type:
  - string
  - 'null'
- description: The classification of the ticket. 'problem' tickets can have linked 'incident' tickets. 'task' tickets support due dates.
  name: type
  type:
  - string
  - 'null'
- description: The subject line of the ticket, typically a brief summary of the issue.
  name: subject
  type: string
- description: The original subject as entered by the requester, before any processing by Zendesk.
  name: raw_subject
  type: string
- description: The first comment on the ticket, set at creation time. Read-only after the ticket is created.
  name: description
  type: string
- description: The urgency level of the ticket.
  name: priority
  type:
  - string
  - 'null'
- description: The current state of the ticket in its lifecycle.
  name: status
  type: string
- description: The original recipient email address of the ticket.
  name: recipient
  type:
  - string
  - 'null'
- description: The ID of the user who requested the ticket (the customer).
  name: requester_id
  type: integer
- description: The ID of the user who submitted the ticket. Can differ from the requester when an agent creates a ticket on behalf of a customer.
  name: submitter_id
  type: integer
- description: The ID of the agent currently assigned to the ticket.
  name: assignee_id
  type:
  - integer
  - 'null'
- description: The ID of the organization associated with the ticket.
  name: organization_id
  type:
  - integer
  - 'null'
- description: The ID of the agent group assigned to the ticket.
  name: group_id
  type:
  - integer
  - 'null'
- description: IDs of users currently CC'd on the ticket.
  name: collaborator_ids
  type: array
- description: IDs of agents currently following the ticket for internal notifications.
  name: follower_ids
  type: array
- description: IDs of agents or end users currently CC'd on the ticket via email.
  name: email_cc_ids
  type: array
- description: The ID of the associated community forum topic, if the ticket originated from a forum post.
  name: forum_topic_id
  type:
  - integer
  - 'null'
- description: For incident tickets, the ID of the problem ticket this incident is linked to.
  name: problem_id
  type:
  - integer
  - 'null'
- description: Whether this problem ticket has associated incident tickets.
  name: has_incidents
  type: boolean
- description: Whether the ticket has any public-facing comments.
  name: is_public
  type: boolean
- description: The due date for task-type tickets, in ISO 8601 format.
  name: due_at
  type:
  - string
  - 'null'
- description: Tags applied to the ticket for categorization and routing.
  name: tags
  type: array
- description: Custom field values set on the ticket.
  name: custom_fields
  type: array
- description: The satisfaction rating left by the customer, if any.
  name: satisfaction_rating
  type:
  - object
  - 'null'
- description: IDs of sharing agreements used for the ticket.
  name: sharing_agreement_ids
  type: array
- description: The ID of the custom ticket status, if custom statuses are enabled.
  name: custom_status_id
  type:
  - integer
  - 'null'
- description: IDs of follow-up tickets created from this closed ticket.
  name: followup_ids
  type: array
- description: The ID of the ticket form used for this ticket.
  name: ticket_form_id
  type:
  - integer
  - 'null'
- description: The ID of the brand associated with this ticket.
  name: brand_id
  type:
  - integer
  - 'null'
- description: Whether channelback is enabled for this ticket.
  name: allow_channelback
  type: boolean
- description: Whether the ticket allows file attachments.
  name: allow_attachments
  type: boolean
- description: Whether the ticket originated from a messaging channel.
  name: from_messaging_channel
  type: boolean
- description: How the ticket was created (e.g., web, email, API, chat).
  name: via
  type: object
- description: When the ticket was created, in ISO 8601 format.
  name: created_at
  type: string
- description: When the ticket was last updated, in ISO 8601 format.
  name: updated_at
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-ticket-schema.json
slug: zendesk-ticket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-ticket-schema.json\",\n  \"title\": \"Zendesk Ticket\",\n  \"description\": \"A Zendesk Support ticket representing a customer service request. Tickets are the core entity in Zendesk Support, capturing the communication between a customer and support agents. Each ticket has a lifecycle from creation through resolution, with statuses, priorities, assignees, and a full audit trail of changes and comments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Automatically assigned unique identifier for the ticket.\",\n      \"readOnly\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL of the ticket resource.\",\n      \"readOnly\": true\n\
  \    },\n    \"external_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional ID from an external system used to link the ticket to records outside Zendesk.\"\n    },\n    \"type\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"problem\", \"incident\", \"question\", \"task\", null],\n      \"description\": \"The classification of the ticket. 'problem' tickets can have linked 'incident' tickets. 'task' tickets support due dates.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"maxLength\": 150,\n      \"description\": \"The subject line of the ticket, typically a brief summary of the issue.\"\n    },\n    \"raw_subject\": {\n      \"type\": \"string\",\n      \"description\": \"The original subject as entered by the requester, before any processing by Zendesk.\",\n      \"readOnly\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The first comment on the ticket, set at creation\
  \ time. Read-only after the ticket is created.\",\n      \"readOnly\": true\n    },\n    \"priority\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"urgent\", \"high\", \"normal\", \"low\", null],\n      \"description\": \"The urgency level of the ticket.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"new\", \"open\", \"pending\", \"hold\", \"solved\", \"closed\"],\n      \"description\": \"The current state of the ticket in its lifecycle.\"\n    },\n    \"recipient\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The original recipient email address of the ticket.\",\n      \"readOnly\": true\n    },\n    \"requester_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The ID of the user who requested the ticket (the customer).\"\n    },\n    \"submitter_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\":\
  \ \"The ID of the user who submitted the ticket. Can differ from the requester when an agent creates a ticket on behalf of a customer.\",\n      \"readOnly\": true\n    },\n    \"assignee_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the agent currently assigned to the ticket.\"\n    },\n    \"organization_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the organization associated with the ticket.\"\n    },\n    \"group_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the agent group assigned to the ticket.\"\n    },\n    \"collaborator_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"IDs of users currently CC'd on the ticket.\"\n    },\n    \"follower_ids\": {\n      \"type\": \"\
  array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"IDs of agents currently following the ticket for internal notifications.\",\n      \"readOnly\": true\n    },\n    \"email_cc_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"IDs of agents or end users currently CC'd on the ticket via email.\"\n    },\n    \"forum_topic_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the associated community forum topic, if the ticket originated from a forum post.\",\n      \"readOnly\": true\n    },\n    \"problem_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"For incident tickets, the ID of the problem ticket this incident is linked to.\"\n    },\n    \"has_incidents\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether this problem ticket has associated incident tickets.\",\n      \"readOnly\": true\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket has any public-facing comments.\",\n      \"readOnly\": true\n    },\n    \"due_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The due date for task-type tickets, in ISO 8601 format.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags applied to the ticket for categorization and routing.\"\n    },\n    \"custom_fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomField\"\n      },\n      \"description\": \"Custom field values set on the ticket.\"\n    },\n    \"satisfaction_rating\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The satisfaction rating\
  \ left by the customer, if any.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"score\": {\n          \"type\": \"string\",\n          \"enum\": [\"offered\", \"unoffered\", \"good\", \"bad\"]\n        },\n        \"comment\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"sharing_agreement_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"IDs of sharing agreements used for the ticket.\",\n      \"readOnly\": true\n    },\n    \"custom_status_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the custom ticket status, if custom statuses are enabled.\"\n    },\n    \"followup_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"IDs of follow-up tickets created from this closed ticket.\"\
  ,\n      \"readOnly\": true\n    },\n    \"ticket_form_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the ticket form used for this ticket.\"\n    },\n    \"brand_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"The ID of the brand associated with this ticket.\"\n    },\n    \"allow_channelback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether channelback is enabled for this ticket.\",\n      \"readOnly\": true\n    },\n    \"allow_attachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket allows file attachments.\",\n      \"readOnly\": true\n    },\n    \"from_messaging_channel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket originated from a messaging channel.\",\n      \"readOnly\": true\n    },\n    \"via\": {\n      \"$ref\": \"#/$defs/Via\",\n      \"description\": \"How the\
  \ ticket was created (e.g., web, email, API, chat).\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the ticket was created, in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the ticket was last updated, in ISO 8601 format.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"id\", \"status\", \"requester_id\"],\n  \"$defs\": {\n    \"CustomField\": {\n      \"type\": \"object\",\n      \"description\": \"A custom field key-value pair on the ticket.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The ID of the custom field.\"\n        },\n        \"value\": {\n          \"description\": \"The value of the custom field.\",\n          \"oneOf\": [\n            { \"type\": \"string\" },\n\
  \            { \"type\": \"number\" },\n            { \"type\": \"boolean\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n            { \"type\": \"null\" }\n          ]\n        }\n      },\n      \"required\": [\"id\", \"value\"]\n    },\n    \"Via\": {\n      \"type\": \"object\",\n      \"description\": \"Describes how the ticket was created or a comment was made.\",\n      \"properties\": {\n        \"channel\": {\n          \"type\": \"string\",\n          \"description\": \"The channel through which the ticket was created (e.g., web, email, api, chat, voice, mobile, closed_ticket, any_channel).\"\n        },\n        \"source\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"from\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true\n            },\n            \"to\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true\n            },\n           \
  \ \"rel\": {\n              \"type\": [\"string\", \"null\"]\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-ticket-schema.json
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
title: Zendesk Ticket
---
