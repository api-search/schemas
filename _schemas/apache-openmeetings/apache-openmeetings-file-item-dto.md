---
description: FileItemDTO schema from Apache OpenMeetings REST API
layout: schema
name: FileItemDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: hash
  type: string
- description: ''
  name: parentId
  type: integer
- description: ''
  name: roomId
  type: integer
- description: ''
  name: groupId
  type: integer
- description: ''
  name: ownerId
  type: integer
- description: ''
  name: size
  type: integer
- description: ''
  name: externalId
  type: string
- description: ''
  name: externalType
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: width
  type: integer
- description: ''
  name: height
  type: integer
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-file-item-dto-schema.json
slug: apache-openmeetings-file-item-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-file-item-dto-schema.json\",\n  \"title\": \"FileItemDTO\",\n  \"description\": \"FileItemDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"hash\": {\n      \"type\": \"string\"\n    },\n    \"parentId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"roomId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"groupId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"ownerId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"format\": \"\
  int64\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"externalType\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"FOLDER\",\n        \"IMAGE\",\n        \"POLL_CHART\",\n        \"PRESENTATION\",\n        \"RECORDING\",\n        \"VIDEO\",\n        \"WML_FILE\"\n      ]\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-file-item-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: FileItemDTO
---
