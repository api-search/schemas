---
description: ''
layout: schema
name: Workspace
properties_list:
- description: The creation date
  name: createdAt
  type: string
- description: The default ttl for the workspaces items, in seconds. If not set, the default will be set by server configuration (currently 1 year)
  name: defaultItemTtl
  type: number
- description: ''
  name: id
  type: object
- description: A list of user defined labels or tags
  name: labels
  type: array
- description: The name of the workspace, must be seen as a human readable technique id. Can not be formatted like an id. Must be unique in the platform. Auto-generated if not provided at the creation of the workspa
  name: name
  type: string
- description: Human readable workspace title for convenience
  name: title
  type: string
- description: The id of the user who own the workspace
  name: userId
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-workspace-schema.json
slug: oneatlas-workspace
source_filename: oneatlas-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-schema.json\",\n  \"title\": \"Workspace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"The creation date\",\n      \"example\": \"2017-10-12T08:55:52.651155Z\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"defaultItemTtl\": {\n      \"description\": \"The default ttl for the workspaces items, in seconds. If not set, the default will be set by server configuration (currently 1 year)\",\n      \"example\": 123456,\n      \"format\": \"int\",\n      \"type\": \"number\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"labels\": {\n      \"description\": \"A list of user defined labels or tags\",\n      \"example\": [\n        \"p\\u00eache\",\n \
  \       \"lac de biscarosse\",\n        \"carpe\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The name of the workspace, must be seen as a human readable technique id. Can not be formatted like an id. Must be unique in the platform. Auto-generated if not provided at the creation of the workspace.\",\n      \"example\": \"flyinghippo\",\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"description\": \"Human readable workspace title for convenience\",\n      \"example\": \"S2 items\",\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"description\": \"The id of the user who own the workspace\",\n      \"example\": \"aEr5695feGGn0ob\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-schema.json
tags:
- Imagery
- Satellites
title: Workspace
---
