---
description: ''
layout: schema
name: Registrant
properties_list:
- description: Registrant ID.
  name: id
  type: string
- description: Registrant email address.
  name: email
  type: string
- description: Registrant first name.
  name: first_name
  type: string
- description: Registrant last name.
  name: last_name
  type: string
- description: ''
  name: address
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zip
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: industry
  type: string
- description: ''
  name: org
  type: string
- description: ''
  name: job_title
  type: string
- description: ''
  name: purchasing_time_frame
  type: string
- description: ''
  name: role_in_purchase_process
  type: string
- description: ''
  name: no_of_employees
  type: string
- description: ''
  name: comments
  type: string
- description: Registrant status.
  name: status
  type: string
- description: Time the registrant registered.
  name: create_time
  type: string
- description: Unique join URL for this registrant.
  name: join_url
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-registrant-schema.json
slug: zoom-meeting-registrant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Registrant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant ID.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant email address.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant first name.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant last name.\"\n    },\n    \"address\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"zip\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"industry\": {\n      \"type\": \"string\"\n    },\n    \"org\": {\n      \"type\": \"string\"\
  \n    },\n    \"job_title\": {\n      \"type\": \"string\"\n    },\n    \"purchasing_time_frame\": {\n      \"type\": \"string\"\n    },\n    \"role_in_purchase_process\": {\n      \"type\": \"string\"\n    },\n    \"no_of_employees\": {\n      \"type\": \"string\"\n    },\n    \"comments\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant status.\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time the registrant registered.\"\n    },\n    \"join_url\": {\n      \"type\": \"string\",\n      \"description\": \"Unique join URL for this registrant.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-registrant-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: Registrant
---
