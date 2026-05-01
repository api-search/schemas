---
description: A support or service desk ticket common across Freshdesk and Freshservice products. Tickets represent customer or employee requests for assistance, incidents, or service requests.
layout: schema
name: Freshworks Ticket
properties_list:
- description: Unique identifier of the ticket.
  name: id
  type: integer
- description: Subject line summarizing the ticket request.
  name: subject
  type: string
- description: HTML-formatted description of the ticket with full details of the request.
  name: description
  type: string
- description: Plain text version of the ticket description.
  name: description_text
  type: string
- description: Numeric status code. 2=Open, 3=Pending, 4=Resolved, 5=Closed.
  name: status
  type: integer
- description: Numeric priority level. 1=Low, 2=Medium, 3=High, 4=Urgent.
  name: priority
  type: integer
- description: Category type of the ticket (e.g., Question, Incident, Problem, Feature Request, Service Request).
  name: type
  type: string
- description: Source channel through which the ticket was created. 1=Email, 2=Portal, 3=Phone, 7=Chat, 9=Feedback Widget, 10=Outbound Email.
  name: source
  type: integer
- description: ID of the requester (contact or employee) who raised the ticket.
  name: requester_id
  type: integer
- description: Email address of the requester.
  name: requester_email
  type: string
- description: ID of the agent assigned to handle the ticket.
  name: responder_id
  type: integer
- description: ID of the agent group to which the ticket is assigned.
  name: group_id
  type: integer
- description: ID of the associated company (Freshdesk) or department (Freshservice).
  name: company_id
  type: integer
- description: ID of the product or service associated with the ticket.
  name: product_id
  type: integer
- description: Labels or tags applied to the ticket for categorization.
  name: tags
  type: array
- description: Timestamp by which the ticket should be resolved.
  name: due_by
  type: string
- description: Timestamp by which the first response to the ticket is due.
  name: fr_due_by
  type: string
- description: Indicates whether the ticket has been escalated due to SLA breach.
  name: is_escalated
  type: boolean
- description: Key-value pairs containing custom field data specific to the helpdesk configuration.
  name: custom_fields
  type: object
- description: File attachments associated with the ticket.
  name: attachments
  type: array
- description: Timestamp when the ticket was created.
  name: created_at
  type: string
- description: Timestamp when the ticket was last updated.
  name: updated_at
  type: string
provider_name: freshworks
provider_slug: freshworks
schema_file: json-schema/freshworks-ticket-schema.json
slug: freshworks-ticket
source_filename: freshworks-ticket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://freshworks.com/schemas/freshworks/ticket.json\",\n  \"title\": \"Freshworks Ticket\",\n  \"description\": \"A support or service desk ticket common across Freshdesk and Freshservice products. Tickets represent customer or employee requests for assistance, incidents, or service requests.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"subject\", \"status\", \"priority\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the ticket.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject line summarizing the ticket request.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted description of the ticket with full details of the request.\"\n    },\n    \"description_text\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Plain text version of the ticket description.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric status code. 2=Open, 3=Pending, 4=Resolved, 5=Closed.\",\n      \"enum\": [2, 3, 4, 5]\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric priority level. 1=Low, 2=Medium, 3=High, 4=Urgent.\",\n      \"enum\": [1, 2, 3, 4]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Category type of the ticket (e.g., Question, Incident, Problem, Feature Request, Service Request).\"\n    },\n    \"source\": {\n      \"type\": \"integer\",\n      \"description\": \"Source channel through which the ticket was created. 1=Email, 2=Portal, 3=Phone, 7=Chat, 9=Feedback Widget, 10=Outbound Email.\"\n    },\n    \"requester_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the requester (contact or employee) who raised the ticket.\"\
  \n    },\n    \"requester_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the requester.\"\n    },\n    \"responder_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the agent assigned to handle the ticket.\"\n    },\n    \"group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the agent group to which the ticket is assigned.\"\n    },\n    \"company_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the associated company (Freshdesk) or department (Freshservice).\"\n    },\n    \"product_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the product or service associated with the ticket.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Labels or tags applied to the ticket for categorization.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"due_by\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"date-time\",\n      \"description\": \"Timestamp by which the ticket should be resolved.\"\n    },\n    \"fr_due_by\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp by which the first response to the ticket is due.\"\n    },\n    \"is_escalated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the ticket has been escalated due to SLA breach.\"\n    },\n    \"custom_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs containing custom field data specific to the helpdesk configuration.\",\n      \"additionalProperties\": true\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"File attachments associated with the ticket.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Attachment\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when\
  \ the ticket was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the ticket was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Attachment\": {\n      \"type\": \"object\",\n      \"description\": \"A file attachment on a ticket.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique ID of the attachment.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"File name of the attachment.\"\n        },\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the attachment.\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"File size in bytes.\"\n        },\n        \"attachment_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to\
  \ download the attachment.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the attachment was uploaded.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/json-schema/freshworks-ticket-schema.json
tags: []
title: Freshworks Ticket
---
