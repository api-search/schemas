---
description: GroupDTOListWrapper schema from Apache OpenMeetings REST API
layout: schema
name: GroupDTOListWrapper
properties_list:
- description: ''
  name: groupDTO
  type: array
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-group-dto-list-wrapper-schema.json
slug: apache-openmeetings-group-dto-list-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-group-dto-list-wrapper-schema.json\",\n  \"title\": \"GroupDTOListWrapper\",\n  \"description\": \"GroupDTOListWrapper schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupDTO\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GroupDTO\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-group-dto-list-wrapper-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: GroupDTOListWrapper
---
