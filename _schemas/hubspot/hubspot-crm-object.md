---
description: Schema for a HubSpot CRM object record, applicable to contacts, companies, deals, tickets, and other CRM object types.
layout: schema
name: HubSpot CRM Object
properties_list:
- description: The unique identifier for the CRM object record assigned by HubSpot.
  name: id
  type: string
- description: The CRM object's properties as key-value pairs. Keys are property names and values are the property values as strings.
  name: properties
  type: object
- description: A map of property names to their historical values, including the current value and previous values with timestamps.
  name: propertiesWithHistory
  type: object
- description: The date and time the CRM object record was created in ISO 8601 format.
  name: createdAt
  type: string
- description: The date and time the CRM object record was last updated in ISO 8601 format.
  name: updatedAt
  type: string
- description: Whether the CRM object record has been archived (soft deleted). Archived records can be restored.
  name: archived
  type: boolean
- description: The date and time the CRM object record was archived, if applicable.
  name: archivedAt
  type: string
- description: Associations between this CRM object and other CRM objects, keyed by object type.
  name: associations
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-object-schema.json
slug: hubspot-crm-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.hubspot.com/docs/api/schemas/crm-object\",\n  \"title\": \"HubSpot CRM Object\",\n  \"description\": \"Schema for a HubSpot CRM object record, applicable to contacts, companies, deals, tickets, and other CRM object types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the CRM object record assigned by HubSpot.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The CRM object's properties as key-value pairs. Keys are property names and values are the property values as strings.\",\n      \"additionalProperties\": {\n        \"type\": [\"string\", \"null\"],\n        \"description\": \"A property value for the CRM object.\"\n      },\n      \"examples\": [\n        {\n          \"firstname\": \"John\",\n          \"lastname\": \"Doe\",\n      \
  \    \"email\": \"john.doe@example.com\",\n          \"phone\": \"+1-555-555-5555\",\n          \"company\": \"Acme Corp\"\n        }\n      ]\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"object\",\n      \"description\": \"A map of property names to their historical values, including the current value and previous values with timestamps.\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/$defs/PropertyHistory\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the CRM object record was created in ISO 8601 format.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the CRM object record was last updated in ISO 8601 format.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the CRM object record has been archived (soft deleted). Archived records can be restored.\",\n      \"default\": false\n    },\n    \"archivedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the CRM object record was archived, if applicable.\"\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"description\": \"Associations between this CRM object and other CRM objects, keyed by object type.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AssociationCollection\"\n      },\n      \"examples\": [\n        {\n          \"companies\": {\n            \"results\": [\n              { \"id\": \"789\", \"type\": \"contact_to_company\" }\n            ]\n          },\n          \"deals\": {\n            \"results\": [\n              { \"id\": \"456\", \"type\": \"contact_to_deal\" }\n            ]\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\"id\", \"properties\", \"createdAt\"\
  , \"updatedAt\"],\n  \"$defs\": {\n    \"PropertyHistory\": {\n      \"type\": \"object\",\n      \"description\": \"A historical value entry for a CRM property.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The value of the property at the given timestamp.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when this property value was set.\"\n        },\n        \"sourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The source type that set this property value (e.g., CRM_UI, API, IMPORT).\"\n        },\n        \"sourceId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The source ID that set this property value.\"\n        }\n      },\n      \"required\": [\"value\", \"timestamp\"]\n    },\n    \"Association\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"An association between two CRM object records.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the associated CRM object record.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The association type label describing the relationship.\"\n        }\n      },\n      \"required\": [\"id\", \"type\"]\n    },\n    \"AssociationCollection\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of associations to a specific object type.\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"description\": \"The list of associated records.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Association\"\n          }\n        },\n        \"paging\": {\n          \"$ref\": \"#/$defs/Paging\"\n        }\n      },\n      \"required\": [\"results\"]\n    },\n    \"Paging\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Pagination information for a collection response.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Information for fetching the next page of results.\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"The cursor token to use in the 'after' parameter to get the next page.\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"A direct URL link to the next page of results.\"\n            }\n          },\n          \"required\": [\"after\"]\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": \"1234\",\n      \"properties\": {\n        \"firstname\": \"Jane\",\n        \"lastname\": \"Smith\",\n        \"email\": \"jane.smith@example.com\",\n        \"phone\": \"+1-555-123-4567\",\n        \"company\"\
  : \"Example Corp\",\n        \"hs_object_id\": \"1234\"\n      },\n      \"createdAt\": \"2023-01-15T10:30:00Z\",\n      \"updatedAt\": \"2024-06-20T14:45:00Z\",\n      \"archived\": false,\n      \"associations\": {\n        \"companies\": {\n          \"results\": [\n            { \"id\": \"5678\", \"type\": \"contact_to_company\" }\n          ]\n        }\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-object-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: HubSpot CRM Object
---
