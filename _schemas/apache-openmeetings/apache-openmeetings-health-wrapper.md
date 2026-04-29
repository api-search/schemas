---
description: HealthWrapper schema from Apache OpenMeetings REST API
layout: schema
name: HealthWrapper
properties_list:
- description: ''
  name: health
  type: object
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-health-wrapper-schema.json
slug: apache-openmeetings-health-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-health-wrapper-schema.json\",\n  \"title\": \"HealthWrapper\",\n  \"description\": \"HealthWrapper schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"health\": {\n      \"$ref\": \"#/components/schemas/Health\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-health-wrapper-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: HealthWrapper
---
