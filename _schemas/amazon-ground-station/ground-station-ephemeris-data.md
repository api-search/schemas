---
description: Ephemeris data.
layout: schema
name: EphemerisData
properties_list:
- description: ''
  name: oem
  type: object
- description: ''
  name: tle
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ephemeris-data-schema.json
slug: ground-station-ephemeris-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-data-schema.json\",\n  \"title\": \"EphemerisData\",\n  \"description\": \"Ephemeris data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"oem\": {\n      \"$ref\": \"#/components/schemas/OEMEphemeris\"\n    },\n    \"tle\": {\n      \"$ref\": \"#/components/schemas/TLEEphemeris\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EphemerisData
---
