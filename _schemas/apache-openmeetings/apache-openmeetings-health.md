---
description: Health schema from Apache OpenMeetings REST API
layout: schema
name: Health
properties_list:
- description: ''
  name: inited
  type: boolean
- description: ''
  name: installed
  type: boolean
- description: ''
  name: dbOk
  type: boolean
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-health-schema.json
slug: apache-openmeetings-health
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-health-schema.json\",\n  \"title\": \"Health\",\n  \"description\": \"Health schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inited\": {\n      \"type\": \"boolean\"\n    },\n    \"installed\": {\n      \"type\": \"boolean\"\n    },\n    \"dbOk\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-health-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: Health
---
