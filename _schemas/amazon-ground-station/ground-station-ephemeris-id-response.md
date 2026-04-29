---
description: EphemerisIdResponse schema from Amazon Ground Station API
layout: schema
name: EphemerisIdResponse
properties_list:
- description: ''
  name: ephemerisId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ephemeris-id-response-schema.json
slug: ground-station-ephemeris-id-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-id-response-schema.json\",\n  \"title\": \"EphemerisIdResponse\",\n  \"description\": \"EphemerisIdResponse schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ephemerisId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The AWS Ground Station ephemeris ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-id-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EphemerisIdResponse
---
