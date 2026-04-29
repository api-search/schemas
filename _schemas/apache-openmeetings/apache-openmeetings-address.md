---
description: Address schema from Apache OpenMeetings REST API
layout: schema
name: Address
properties_list:
- description: ''
  name: inserted
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: deleted
  type: boolean
- description: ''
  name: id
  type: integer
- description: ''
  name: additionalname
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: fax
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: street
  type: string
- description: ''
  name: town
  type: string
- description: ''
  name: zip
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-address-schema.json
slug: apache-openmeetings-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inserted\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"xml\": {\n        \"name\": \"created\"\n      }\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"additionalname\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"fax\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"street\"\
  : {\n      \"type\": \"string\"\n    },\n    \"town\": {\n      \"type\": \"string\"\n    },\n    \"zip\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"xml\": {\n        \"name\": \"mail\"\n      }\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-address-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: Address
---
