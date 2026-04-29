---
description: Represents a webhook event payload delivered by the Autodesk Webhooks API to registered callback URLs when events occur in Data Management, Model Derivative, or other Autodesk systems.
layout: schema
name: Autodesk Webhook Event
properties_list:
- description: The webhook payload schema version.
  name: version
  type: string
- description: The URN of the affected resource.
  name: resourceUrn
  type: string
- description: Information about the webhook subscription that triggered this event.
  name: hook
  type: object
- description: The event-specific payload data.
  name: payload
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-webhook-event.json
slug: autodesk-webhook-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-webhook-event.json\",\n  \"title\": \"Autodesk Webhook Event\",\n  \"description\": \"Represents a webhook event payload delivered by the Autodesk Webhooks API to registered callback URLs when events occur in Data Management, Model Derivative, or other Autodesk systems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The webhook payload schema version.\"\n    },\n    \"resourceUrn\": {\n      \"type\": \"string\",\n      \"description\": \"The URN of the affected resource.\"\n    },\n    \"hook\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the webhook subscription that triggered this event.\",\n      \"properties\": {\n        \"hookId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Unique hook identifier.\"\n        },\n        \"tenant\": {\n          \"type\": \"string\",\n          \"description\": \"The application client ID.\"\n        },\n        \"callbackUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL the event was delivered to.\"\n        },\n        \"createdBy\": {\n          \"type\": \"string\"\n        },\n        \"event\": {\n          \"type\": \"string\",\n          \"description\": \"The event type that triggered the callback.\",\n          \"examples\": [\n            \"dm.version.added\",\n            \"dm.version.deleted\",\n            \"dm.version.modified\",\n            \"dm.folder.added\",\n            \"dm.folder.deleted\",\n            \"extraction.finished\",\n            \"extraction.updated\",\n            \"model.sync.publish\"\n          ]\n        },\n        \"createdDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n \
  \       \"system\": {\n          \"type\": \"string\",\n          \"description\": \"The event system.\",\n          \"examples\": [\"data\", \"derivative\", \"adsk.c4r\", \"adsk.docs\"]\n        },\n        \"creatorType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Application\", \"O2User\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"inactive\"]\n        },\n        \"scope\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"folder\": {\n              \"type\": \"string\"\n            },\n            \"workflow\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"hookAttribute\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Custom metadata attached to the subscription.\"\n        }\n      },\n      \"required\": [\"hookId\", \"event\", \"system\"]\n    },\n    \"payload\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"The event-specific payload data.\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"project\": {\n          \"type\": \"string\",\n          \"description\": \"Project ID.\"\n        },\n        \"creator\": {\n          \"type\": \"string\",\n          \"description\": \"User ID who triggered the event.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the affected resource.\"\n        },\n        \"lineageUrn\": {\n          \"type\": \"string\",\n          \"description\": \"The lineage URN of the item.\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Processing status (for derivative events).\"\n        },\n        \"createdTime\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\"\n        },\n        \"modifiedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  },\n  \"required\": [\"version\", \"resourceUrn\", \"hook\", \"payload\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-webhook-event.json
tags:
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
title: Autodesk Webhook Event
---
