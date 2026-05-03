---
description: A Rollbar item representing a unique error or message tracked by Rollbar, grouped by fingerprint. Items are the primary unit of work in Rollbar's error tracking workflow.
layout: schema
name: Rollbar Item
properties_list:
- description: The internal item ID used for API operations.
  name: id
  type: integer
- description: The project-specific counter displayed in Rollbar URLs (e.g., items/456).
  name: counter
  type: integer
- description: The environment where this item was first seen (e.g., production, staging).
  name: environment
  type: string
- description: Framework identifier code representing the application framework.
  name: framework
  type: integer
- description: The fingerprint hash used to group occurrences into this item.
  name: hash
  type: string
- description: The title or summary of the item, typically derived from the error message.
  name: title
  type: string
- description: The instance ID of the first occurrence of this item.
  name: first_occurrence_id
  type: integer
- description: Unix timestamp when this item was first seen.
  name: first_occurrence_timestamp
  type: integer
- description: The instance ID of the most recent occurrence of this item.
  name: last_occurrence_id
  type: integer
- description: Unix timestamp of the most recent occurrence.
  name: last_occurrence_timestamp
  type: integer
- description: The severity level of the item.
  name: level
  type: string
- description: The current workflow status of the item.
  name: status
  type: string
- description: Total number of times this item has occurred.
  name: total_occurrences
  type: integer
- description: Number of unique occurrences based on deduplication criteria.
  name: unique_occurrences
  type: integer
- description: The project ID this item belongs to.
  name: project_id
  type: integer
- description: The code version in which this item was resolved.
  name: resolved_in_version
  type:
  - string
  - 'null'
- description: The user ID of the person assigned to investigate this item.
  name: assigned_user_id
  type:
  - integer
  - 'null'
- description: Data from third-party integrations linked to this item.
  name: integrations_data
  type: object
- description: Unix timestamp when the item was last activated or reactivated.
  name: last_activated_timestamp
  type: integer
- description: Unix timestamp when the item was last resolved.
  name: last_resolved_timestamp
  type:
  - integer
  - 'null'
provider_name: Rollbar
provider_slug: rollbar
schema_file: json-schema/rollbar-item-schema.json
slug: rollbar-item
source_filename: rollbar-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rollbar.com/schemas/rollbar/item.json\",\n  \"title\": \"Rollbar Item\",\n  \"description\": \"A Rollbar item representing a unique error or message tracked by Rollbar, grouped by fingerprint. Items are the primary unit of work in Rollbar's error tracking workflow.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"counter\", \"title\", \"level\", \"status\", \"project_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal item ID used for API operations.\"\n    },\n    \"counter\": {\n      \"type\": \"integer\",\n      \"description\": \"The project-specific counter displayed in Rollbar URLs (e.g., items/456).\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment where this item was first seen (e.g., production, staging).\",\n      \"maxLength\": 255\n    },\n    \"framework\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Framework identifier code representing the application framework.\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"The fingerprint hash used to group occurrences into this item.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title or summary of the item, typically derived from the error message.\"\n    },\n    \"first_occurrence_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The instance ID of the first occurrence of this item.\"\n    },\n    \"first_occurrence_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when this item was first seen.\"\n    },\n    \"last_occurrence_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The instance ID of the most recent occurrence of this item.\"\n    },\n    \"last_occurrence_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp\
  \ of the most recent occurrence.\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the item.\",\n      \"enum\": [\"critical\", \"error\", \"warning\", \"info\", \"debug\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current workflow status of the item.\",\n      \"enum\": [\"active\", \"resolved\", \"muted\"]\n    },\n    \"total_occurrences\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of times this item has occurred.\",\n      \"minimum\": 0\n    },\n    \"unique_occurrences\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique occurrences based on deduplication criteria.\",\n      \"minimum\": 0\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The project ID this item belongs to.\"\n    },\n    \"resolved_in_version\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The code version\
  \ in which this item was resolved.\",\n      \"maxLength\": 40\n    },\n    \"assigned_user_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The user ID of the person assigned to investigate this item.\"\n    },\n    \"integrations_data\": {\n      \"type\": \"object\",\n      \"description\": \"Data from third-party integrations linked to this item.\"\n    },\n    \"last_activated_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the item was last activated or reactivated.\"\n    },\n    \"last_resolved_timestamp\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Unix timestamp when the item was last resolved.\"\n    }\n  },\n  \"$defs\": {\n    \"ItemLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level for Rollbar items.\",\n      \"enum\": [\"critical\", \"error\", \"warning\", \"info\", \"debug\"]\n    },\n    \"ItemStatus\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"The workflow status for Rollbar items.\",\n      \"enum\": [\"active\", \"resolved\", \"muted\"]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/json-schema/rollbar-item-schema.json
tags:
- Error Tracking
- Monitoring
- Debugging
- DevOps
- Application Performance
title: Rollbar Item
---
