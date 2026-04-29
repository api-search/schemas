---
description: Request body for creating a membership.
layout: schema
name: CreateMembershipRequest
properties_list:
- description: The unique ID for the associated collaboration.
  name: collaborationIdentifier
  type: string
- description: An indicator as to whether query logging has been enabled or disabled.
  name: queryLogStatus
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-create-membership-request-schema.json
slug: clean-rooms-create-membership-request
source_filename: clean-rooms-create-membership-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-membership-request-schema.json\",\n  \"title\": \"CreateMembershipRequest\",\n  \"description\": \"Request body for creating a membership.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"collaborationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID for the associated collaboration.\",\n      \"example\": \"collab-abc12345\"\n    },\n    \"queryLogStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"An indicator as to whether query logging has been enabled or disabled.\"\n    }\n  },\n  \"required\": [\n    \"collaborationIdentifier\",\n    \"queryLogStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-membership-request-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: CreateMembershipRequest
---
