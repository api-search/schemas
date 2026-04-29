---
description: <p/>
layout: schema
name: ListContactsRequest
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: groundStation
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: missionProfileArn
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: satelliteArn
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: statusList
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-contacts-request-schema.json
slug: ground-station-list-contacts-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-contacts-request-schema.json\",\n  \"title\": \"ListContactsRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"End time of a contact in UTC.\"\n        }\n      ]\n    },\n    \"groundStation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationName\"\n        },\n        {\n          \"description\": \"Name of a ground station.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationMaxResults\"\n        },\n        {\n          \"description\": \"Maximum number of\
  \ contacts returned.\"\n        }\n      ]\n    },\n    \"missionProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MissionProfileArn\"\n        },\n        {\n          \"description\": \"ARN of a mission profile.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Next token returned in the request of a previous <code>ListContacts</code> call. Used to get the next page of results.\"\n        }\n      ]\n    },\n    \"satelliteArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/satelliteArn\"\n        },\n        {\n          \"description\": \"ARN of a satellite.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Start time of a contact\
  \ in UTC.\"\n        }\n      ]\n    },\n    \"statusList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusList\"\n        },\n        {\n          \"description\": \"Status of a contact reservation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"startTime\",\n    \"statusList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-contacts-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListContactsRequest
---
