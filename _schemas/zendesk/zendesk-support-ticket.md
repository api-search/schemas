---
description: A Zendesk Support ticket representing a customer service request.
layout: schema
name: Ticket
properties_list:
- description: Automatically assigned ticket ID.
  name: id
  type: integer
- description: The API URL of the ticket.
  name: url
  type: string
- description: An ID from an external system.
  name: external_id
  type: string
- description: The type of the ticket.
  name: type
  type: string
- description: The subject of the ticket.
  name: subject
  type: string
- description: The original subject of the ticket as entered by the requester.
  name: raw_subject
  type: string
- description: The first comment on the ticket (read-only after creation).
  name: description
  type: string
- description: The urgency of the ticket.
  name: priority
  type: string
- description: The current status of the ticket.
  name: status
  type: string
- description: The original recipient email address of the ticket.
  name: recipient
  type: string
- description: The ID of the user who requested the ticket.
  name: requester_id
  type: integer
- description: The ID of the user who submitted the ticket.
  name: submitter_id
  type: integer
- description: The ID of the agent assigned to the ticket.
  name: assignee_id
  type: integer
- description: The ID of the organization associated with the ticket.
  name: organization_id
  type: integer
- description: The ID of the group assigned to the ticket.
  name: group_id
  type: integer
- description: IDs of users currently CC'd on the ticket.
  name: collaborator_ids
  type: array
- description: IDs of agents currently following the ticket.
  name: follower_ids
  type: array
- description: IDs of agents or end users currently CC'd on the ticket.
  name: email_cc_ids
  type: array
- description: The ID of the topic in the community forum, if applicable.
  name: forum_topic_id
  type: integer
- description: For incident tickets, the ID of the associated problem ticket.
  name: problem_id
  type: integer
- description: Whether the ticket has been marked as a problem with incidents.
  name: has_incidents
  type: boolean
- description: Whether the ticket has a public comment.
  name: is_public
  type: boolean
- description: The due date for task tickets (ISO 8601).
  name: due_at
  type: string
- description: Tags applied to the ticket.
  name: tags
  type: array
- description: Custom field key-value pairs.
  name: custom_fields
  type: array
- description: The satisfaction rating of the ticket, if rated.
  name: satisfaction_rating
  type: object
- description: IDs of sharing agreements used for the ticket.
  name: sharing_agreement_ids
  type: array
- description: The ID of a custom ticket status.
  name: custom_status_id
  type: integer
- description: Custom field values (alias for custom_fields).
  name: fields
  type: array
- description: IDs of follow-up tickets created from this ticket.
  name: followup_ids
  type: array
- description: The ID of the ticket form used for this ticket.
  name: ticket_form_id
  type: integer
- description: The ID of the brand this ticket is associated with.
  name: brand_id
  type: integer
- description: Whether channelback is enabled.
  name: allow_channelback
  type: boolean
- description: Whether the ticket allows attachments.
  name: allow_attachments
  type: boolean
- description: Whether the ticket originated from a messaging channel.
  name: from_messaging_channel
  type: boolean
- description: When the ticket was created (ISO 8601).
  name: created_at
  type: string
- description: When the ticket was last updated (ISO 8601).
  name: updated_at
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-ticket-schema.json
slug: zendesk-support-ticket
source_filename: zendesk-support-ticket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ticket\",\n  \"type\": \"object\",\n  \"description\": \"A Zendesk Support ticket representing a customer service request.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Automatically assigned ticket ID.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The API URL of the ticket.\"\n    },\n    \"external_id\": {\n      \"type\": \"string\",\n      \"description\": \"An ID from an external system.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the ticket.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the ticket.\"\n    },\n    \"raw_subject\": {\n      \"type\": \"string\",\n      \"description\": \"The original subject of the ticket as entered by the requester.\"\n    },\n    \"description\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The first comment on the ticket (read-only after creation).\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"The urgency of the ticket.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the ticket.\"\n    },\n    \"recipient\": {\n      \"type\": \"string\",\n      \"description\": \"The original recipient email address of the ticket.\"\n    },\n    \"requester_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user who requested the ticket.\"\n    },\n    \"submitter_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user who submitted the ticket.\"\n    },\n    \"assignee_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the agent assigned to the ticket.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the organization associated\
  \ with the ticket.\"\n    },\n    \"group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the group assigned to the ticket.\"\n    },\n    \"collaborator_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of users currently CC'd on the ticket.\"\n    },\n    \"follower_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of agents currently following the ticket.\"\n    },\n    \"email_cc_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of agents or end users currently CC'd on the ticket.\"\n    },\n    \"forum_topic_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the topic in the community forum, if applicable.\"\n    },\n    \"problem_id\": {\n      \"type\": \"integer\",\n      \"description\": \"For incident tickets, the ID of the associated problem ticket.\"\n    },\n    \"has_incidents\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket has been marked as\
  \ a problem with incidents.\"\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket has a public comment.\"\n    },\n    \"due_at\": {\n      \"type\": \"string\",\n      \"description\": \"The due date for task tickets (ISO 8601).\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the ticket.\"\n    },\n    \"custom_fields\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field key-value pairs.\"\n    },\n    \"satisfaction_rating\": {\n      \"type\": \"object\",\n      \"description\": \"The satisfaction rating of the ticket, if rated.\"\n    },\n    \"sharing_agreement_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of sharing agreements used for the ticket.\"\n    },\n    \"custom_status_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of a custom ticket status.\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Custom field values (alias for custom_fields).\"\n    },\n    \"followup_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of follow-up tickets created from this ticket.\"\n    },\n    \"ticket_form_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the ticket form used for this ticket.\"\n    },\n    \"brand_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the brand this ticket is associated with.\"\n    },\n    \"allow_channelback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether channelback is enabled.\"\n    },\n    \"allow_attachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket allows attachments.\"\n    },\n    \"from_messaging_channel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket originated from a messaging channel.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the ticket was created\
  \ (ISO 8601).\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the ticket was last updated (ISO 8601).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-ticket-schema.json
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
title: Ticket
---
