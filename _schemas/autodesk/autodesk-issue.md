---
description: Represents a quality issue in BIM 360 or Autodesk Construction Cloud, used for tracking and managing field issues, RFIs, safety observations, and other project-related items.
layout: schema
name: Autodesk Construction Issue
properties_list:
- description: Unique issue identifier.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-issue.json
slug: autodesk-issue
source_filename: autodesk-issue.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-issue.json\",\n  \"title\": \"Autodesk Construction Issue\",\n  \"description\": \"Represents a quality issue in BIM 360 or Autodesk Construction Cloud, used for tracking and managing field issues, RFIs, safety observations, and other project-related items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique issue identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"quality_issues\",\n      \"description\": \"The resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Issue title or summary.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"Detailed issue description.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"open\", \"pending\", \"in_review\", \"closed\", \"void\"],\n          \"description\": \"Current issue status.\"\n        },\n        \"assigned_to\": {\n          \"type\": \"string\",\n          \"description\": \"User ID of the assignee.\"\n        },\n        \"assigned_to_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"user\", \"company\", \"role\"],\n          \"description\": \"Type of entity the issue is assigned to.\"\n        },\n        \"due_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Due date for resolution.\"\n        },\n        \"priority\": {\n          \"type\": \"string\",\n          \"description\": \"Issue priority level.\"\n        },\n        \"location_description\": {\n          \"type\": \"string\",\n          \"description\": \"Text\
  \ description of the issue location.\"\n        },\n        \"issue_type_id\": {\n          \"type\": \"string\",\n          \"description\": \"The issue type category.\"\n        },\n        \"issue_sub_type_id\": {\n          \"type\": \"string\",\n          \"description\": \"The issue sub-type category.\"\n        },\n        \"root_cause_id\": {\n          \"type\": \"string\",\n          \"description\": \"The root cause category.\"\n        },\n        \"target_urn\": {\n          \"type\": \"string\",\n          \"description\": \"URN of the document associated with the issue.\"\n        },\n        \"target_urn_page\": {\n          \"type\": \"string\",\n          \"description\": \"Specific page within the target document.\"\n        },\n        \"starting_version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number where the issue was first identified.\"\n        },\n        \"pushpin_attributes\": {\n          \"type\": \"object\",\n         \
  \ \"description\": \"Pushpin location data for visual issue placement.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\"\n            },\n            \"location\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"x\": { \"type\": \"number\" },\n                \"y\": { \"type\": \"number\" },\n                \"z\": { \"type\": \"number\" }\n              }\n            },\n            \"viewer_state\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"created_by\": {\n          \"type\": \"string\"\n        },\n        \"closed_at\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\":\
  \ \"date-time\"\n        },\n        \"closed_by\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"answer\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The resolution answer.\"\n        },\n        \"comment_count\": {\n          \"type\": \"integer\"\n        },\n        \"attachment_count\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"required\": [\"title\", \"status\"]\n    }\n  },\n  \"required\": [\"id\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-issue.json
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
title: Autodesk Construction Issue
---
