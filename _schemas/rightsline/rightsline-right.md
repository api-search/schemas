---
description: A rights or license record in the Rightsline platform
layout: schema
name: Rightsline Right
properties_list:
- description: Unique rights record identifier
  name: id
  type: string
- description: Associated content or catalog identifier
  name: contentId
  type: string
- description: Rights grantor (licensor)
  name: licensor
  type: string
- description: Rights recipient (licensee)
  name: licensee
  type: string
- description: Territory or region for the rights grant
  name: territory
  type: string
- description: Distribution platform
  name: platform
  type: string
- description: Rights window start date
  name: startDate
  type: string
- description: Rights window end date
  name: endDate
  type: string
- description: Rights record status
  name: status
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
provider_name: Rightsline
provider_slug: rightsline
schema_file: json-schema/rightsline-right-schema.json
slug: rightsline-right
source_filename: rightsline-right-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/rightsline/blob/main/json-schema/rightsline-right-schema.json\",\n  \"title\": \"Rightsline Right\",\n  \"description\": \"A rights or license record in the Rightsline platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique rights record identifier\"\n    },\n    \"contentId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated content or catalog identifier\"\n    },\n    \"licensor\": {\n      \"type\": \"string\",\n      \"description\": \"Rights grantor (licensor)\"\n    },\n    \"licensee\": {\n      \"type\": \"string\",\n      \"description\": \"Rights recipient (licensee)\"\n    },\n    \"territory\": {\n      \"type\": \"string\",\n      \"description\": \"Territory or region for the rights grant\",\n      \"example\": \"US\"\n    },\n    \"platform\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Distribution platform\",\n      \"example\": \"SVOD\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Rights window start date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Rights window end date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Rights record status\",\n      \"enum\": [\"Active\", \"Expired\", \"Pending\", \"Terminated\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"required\": [\"id\", \"contentId\", \"territory\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/json-schema/rightsline-right-schema.json
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
title: Rightsline Right
---
