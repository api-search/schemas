---
description: A ServiceNow service catalog request record representing a user's request for one or more catalog items through the self-service portal.
layout: schema
name: ServiceNow Catalog Request
properties_list:
- description: The unique 32-character system identifier for the request.
  name: sys_id
  type: string
- description: The human-readable request number, prefixed with REQ.
  name: number
  type: string
- description: The current state of the request.
  name: request_state
  type: string
- description: The current stage of the request in the fulfillment workflow.
  name: stage
  type:
  - string
  - 'null'
- description: The user for whom the catalog items were requested.
  name: requested_for
  type: object
- description: The user who submitted the request.
  name: opened_by
  type: object
- description: The date and time the request was submitted.
  name: opened_at
  type: string
- description: The delivery address for physical items.
  name: delivery_address
  type:
  - string
  - 'null'
- description: Special instructions provided by the requester.
  name: special_instructions
  type:
  - string
  - 'null'
- description: The total price for all requested items.
  name: price
  type:
  - string
  - 'null'
- description: The current approval status of the request.
  name: approval
  type:
  - string
  - 'null'
- description: The line items in this request.
  name: requested_items
  type: array
- description: Whether the request is still active.
  name: active
  type: boolean
- description: The date and time the record was created.
  name: sys_created_on
  type: string
- description: The user who created the record.
  name: sys_created_by
  type: string
- description: The date and time the record was last updated.
  name: sys_updated_on
  type: string
- description: The user who last updated the record.
  name: sys_updated_by
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-catalog-request-schema.json
slug: servicenow-catalog-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://servicenow.com/schemas/servicenow/catalog-request.json\",\n  \"title\": \"ServiceNow Catalog Request\",\n  \"description\": \"A ServiceNow service catalog request record representing a user's request for one or more catalog items through the self-service portal.\",\n  \"type\": \"object\",\n  \"required\": [\"sys_id\", \"number\", \"request_state\"],\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-f0-9]{32}$\",\n      \"description\": \"The unique 32-character system identifier for the request.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"pattern\": \"^REQ[0-9]+$\",\n      \"description\": \"The human-readable request number, prefixed with REQ.\"\n    },\n    \"request_state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the request.\"\n    },\n    \"stage\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"The current stage of the request in the fulfillment workflow.\"\n    },\n    \"requested_for\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user for whom the catalog items were requested.\"\n    },\n    \"opened_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who submitted the request.\"\n    },\n    \"opened_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the request was submitted.\"\n    },\n    \"delivery_address\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The delivery address for physical items.\"\n    },\n    \"special_instructions\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Special instructions provided by the requester.\"\n    },\n    \"price\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The total price for all requested items.\"\
  \n    },\n    \"approval\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The current approval status of the request.\"\n    },\n    \"requested_items\": {\n      \"type\": \"array\",\n      \"description\": \"The line items in this request.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RequestedItem\"\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request is still active.\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created.\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the record.\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last updated.\"\n    },\n    \"sys_updated_by\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The user who last updated the record.\"\n    }\n  },\n  \"$defs\": {\n    \"ReferenceField\": {\n      \"type\": [\"object\", \"string\", \"null\"],\n      \"description\": \"A ServiceNow reference field that can be a sys_id string or an object containing a link and value.\",\n      \"properties\": {\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API URL to the referenced record.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The sys_id of the referenced record.\"\n        },\n        \"display_value\": {\n          \"type\": \"string\",\n          \"description\": \"The display value of the referenced record.\"\n        }\n      }\n    },\n    \"RequestedItem\": {\n      \"type\": \"object\",\n      \"description\": \"A requested catalog item within a service catalog request.\",\n      \"properties\": {\n        \"sys_id\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Unique identifier for the requested item.\"\n        },\n        \"number\": {\n          \"type\": \"string\",\n          \"pattern\": \"^RITM[0-9]+$\",\n          \"description\": \"The requested item number, prefixed with RITM.\"\n        },\n        \"cat_item\": {\n          \"$ref\": \"#/$defs/ReferenceField\",\n          \"description\": \"The catalog item that was requested.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The quantity of items requested.\"\n        },\n        \"price\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The price per item.\"\n        },\n        \"stage\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The current fulfillment stage.\"\n        },\n        \"state\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The current state\
  \ of the requested item.\"\n        },\n        \"assigned_to\": {\n          \"$ref\": \"#/$defs/ReferenceField\",\n          \"description\": \"The user assigned to fulfill the item.\"\n        },\n        \"configuration_item\": {\n          \"$ref\": \"#/$defs/ReferenceField\",\n          \"description\": \"The configuration item associated with the request.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-catalog-request-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: ServiceNow Catalog Request
---
