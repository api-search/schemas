---
description: Represents a Webex team that groups people and spaces together for organized collaboration across projects and departments.
layout: schema
name: Cisco Webex Team
properties_list:
- description: Unique identifier for the team.
  name: id
  type: string
- description: A user-friendly name for the team.
  name: name
  type: string
- description: The team's description.
  name: description
  type: string
- description: The person ID of the team creator.
  name: creatorId
  type: string
- description: Date and time the team was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-team-schema.json
slug: cisco-webex-team
source_filename: cisco-webex-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/team.json\",\n  \"title\": \"Cisco Webex Team\",\n  \"description\": \"Represents a Webex team that groups people and spaces together for organized collaboration across projects and departments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the team.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the team.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The team's description.\"\n    },\n    \"creatorId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID of the team creator.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the team was created.\"\n    }\n  },\n\
  \  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-team-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Team
---
