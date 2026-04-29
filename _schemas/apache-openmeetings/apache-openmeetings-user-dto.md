---
description: UserDTO schema from Apache OpenMeetings REST API
layout: schema
name: UserDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: login
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: firstname
  type: string
- description: ''
  name: lastname
  type: string
- description: ''
  name: rights
  type: array
- description: ''
  name: languageId
  type: integer
- description: ''
  name: address
  type: object
- description: ''
  name: timeZoneId
  type: string
- description: ''
  name: externalId
  type: string
- description: ''
  name: externalType
  type: string
- description: ''
  name: pictureUri
  type: string
- description: ''
  name: type
  type: string
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-user-dto-schema.json
slug: apache-openmeetings-user-dto
source_filename: apache-openmeetings-user-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-user-dto-schema.json\",\n  \"title\": \"UserDTO\",\n  \"description\": \"UserDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"login\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"firstname\": {\n      \"type\": \"string\"\n    },\n    \"lastname\": {\n      \"type\": \"string\"\n    },\n    \"rights\": {\n      \"uniqueItems\": true,\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"ADMIN\",\n          \"GROUP_ADMIN\",\n          \"ADMIN_CONFIG\",\n          \"ADMIN_CONNECTIONS\",\n          \"ADMIN_BACKUP\",\n          \"ADMIN_LABEL\"\
  ,\n          \"ROOM\",\n          \"DASHBOARD\",\n          \"LOGIN\",\n          \"SOAP\"\n        ]\n      }\n    },\n    \"languageId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"timeZoneId\": {\n      \"type\": \"string\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"externalType\": {\n      \"type\": \"string\"\n    },\n    \"pictureUri\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"USER\",\n        \"LDAP\",\n        \"OAUTH\",\n        \"EXTERNAL\",\n        \"CONTACT\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-user-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: UserDTO
---
