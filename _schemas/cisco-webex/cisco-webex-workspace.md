---
description: Represents a physical workspace location with Webex devices, including capacity, type, calling, and calendar configurations.
layout: schema
name: Cisco Webex Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Organization ID the workspace belongs to.
  name: orgId
  type: string
- description: Display name of the workspace.
  name: displayName
  type: string
- description: Location ID of the workspace.
  name: workspaceLocationId
  type: string
- description: Floor ID within the location.
  name: floorId
  type: string
- description: Number of people the workspace can accommodate.
  name: capacity
  type: integer
- description: Type of workspace.
  name: type
  type: string
- description: SIP address assigned to the workspace.
  name: sipAddress
  type: string
- description: Calling configuration for the workspace.
  name: calling
  type: object
- description: Calendar configuration for the workspace.
  name: calendar
  type: object
- description: Notes or description for the workspace.
  name: notes
  type: string
- description: Date and time the workspace was created.
  name: created
  type: string
- description: Date and time the workspace was last modified.
  name: lastModified
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-workspace-schema.json
slug: cisco-webex-workspace
source_filename: cisco-webex-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/workspace.json\",\n  \"title\": \"Cisco Webex Workspace\",\n  \"description\": \"Represents a physical workspace location with Webex devices, including capacity, type, calling, and calendar configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workspace.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization ID the workspace belongs to.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the workspace.\"\n    },\n    \"workspaceLocationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location ID of the workspace.\"\n    },\n    \"floorId\": {\n      \"type\": \"string\",\n      \"description\": \"Floor ID within the location.\"\n    },\n    \"capacity\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of people the workspace can accommodate.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of workspace.\",\n      \"enum\": [\"notSet\", \"focus\", \"huddle\", \"meetingRoom\", \"open\", \"desk\", \"other\"]\n    },\n    \"sipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"SIP address assigned to the workspace.\"\n    },\n    \"calling\": {\n      \"type\": \"object\",\n      \"description\": \"Calling configuration for the workspace.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"freeCalling\", \"hybridCalling\", \"webexCalling\", \"webexEdgeForDevices\", \"none\"]\n        },\n        \"hybridCalling\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"emailAddress\": {\n              \"type\": \"string\",\n              \"format\": \"email\"\n            }\n          }\n  \
  \      }\n      }\n    },\n    \"calendar\": {\n      \"type\": \"object\",\n      \"description\": \"Calendar configuration for the workspace.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"google\", \"microsoft\"]\n        },\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        }\n      }\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes or description for the workspace.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the workspace was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the workspace was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-workspace-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Workspace
---
