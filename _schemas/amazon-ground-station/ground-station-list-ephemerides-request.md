---
description: ListEphemeridesRequest schema from Amazon Ground Station API
layout: schema
name: ListEphemeridesRequest
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: satelliteId
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: statusList
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-ephemerides-request-schema.json
slug: ground-station-list-ephemerides-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ephemerides-request-schema.json\",\n  \"title\": \"ListEphemeridesRequest\",\n  \"description\": \"ListEphemeridesRequest schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end time to list in UTC. The operation will return an ephemeris if its expiration time is within the time range defined by the <code>startTime</code> and <code>endTime</code>.\"\n        }\n      ]\n    },\n    \"satelliteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The AWS Ground Station satellite ID to list ephemeris\
  \ for.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time to list in UTC. The operation will return an ephemeris if its expiration time is within the time range defined by the <code>startTime</code> and <code>endTime</code>.\"\n        }\n      ]\n    },\n    \"statusList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisStatusList\"\n        },\n        {\n          \"description\": \"The list of ephemeris status to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"satelliteId\",\n    \"startTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ephemerides-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListEphemeridesRequest
---
