---
description: UserSearchResult schema from Apache OpenMeetings REST API
layout: schema
name: UserSearchResult
properties_list:
- description: ''
  name: objectName
  type: string
- description: ''
  name: records
  type: integer
- description: ''
  name: result
  type: array
- description: ''
  name: errorKey
  type: string
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-user-search-result-schema.json
slug: apache-openmeetings-user-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-user-search-result-schema.json\",\n  \"title\": \"UserSearchResult\",\n  \"description\": \"UserSearchResult schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objectName\": {\n      \"type\": \"string\"\n    },\n    \"records\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserDTO\"\n      }\n    },\n    \"errorKey\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-user-search-result-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: UserSearchResult
---
