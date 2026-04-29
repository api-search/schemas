---
description: FileExplorerObject schema from Apache OpenMeetings REST API
layout: schema
name: FileExplorerObject
properties_list:
- description: ''
  name: userHome
  type: array
- description: ''
  name: roomHome
  type: array
- description: ''
  name: userHomeSize
  type: integer
- description: ''
  name: roomHomeSize
  type: integer
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-file-explorer-object-schema.json
slug: apache-openmeetings-file-explorer-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-file-explorer-object-schema.json\",\n  \"title\": \"FileExplorerObject\",\n  \"description\": \"FileExplorerObject schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userHome\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileItemDTO\"\n      }\n    },\n    \"roomHome\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileItemDTO\"\n      }\n    },\n    \"userHomeSize\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"roomHomeSize\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-file-explorer-object-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: FileExplorerObject
---
