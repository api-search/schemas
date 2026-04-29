---
description: Represents a Webex license for an organization, including total and consumed units and subscription details.
layout: schema
name: Cisco Webex License
properties_list:
- description: Unique identifier for the license.
  name: id
  type: string
- description: Name of the license.
  name: name
  type: string
- description: Total number of license units available.
  name: totalUnits
  type: integer
- description: Number of license units consumed.
  name: consumedUnits
  type: integer
- description: Number of units consumed by users.
  name: consumedByUsers
  type: integer
- description: Number of units consumed by workspaces.
  name: consumedByWorkspaces
  type: integer
- description: Subscription ID associated with the license.
  name: subscriptionId
  type: string
- description: Webex site URL for the license.
  name: siteUrl
  type: string
- description: Type of the Webex site.
  name: siteType
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-license-schema.json
slug: cisco-webex-license
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/license.json\",\n  \"title\": \"Cisco Webex License\",\n  \"description\": \"Represents a Webex license for an organization, including total and consumed units and subscription details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the license.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the license.\"\n    },\n    \"totalUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of license units available.\"\n    },\n    \"consumedUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of license units consumed.\"\n    },\n    \"consumedByUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of units consumed by users.\"\n    },\n    \"consumedByWorkspaces\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Number of units consumed by workspaces.\"\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription ID associated with the license.\"\n    },\n    \"siteUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Webex site URL for the license.\"\n    },\n    \"siteType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the Webex site.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-license-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex License
---
