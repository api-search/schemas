---
description: Two-line element set (TLE) ephemeris.
layout: schema
name: TLEEphemeris
properties_list:
- description: ''
  name: s3Object
  type: object
- description: ''
  name: tleData
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-tle-ephemeris-schema.json
slug: ground-station-tle-ephemeris
source_filename: ground-station-tle-ephemeris-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tle-ephemeris-schema.json\",\n  \"title\": \"TLEEphemeris\",\n  \"description\": \"Two-line element set (TLE) ephemeris.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"Identifies the S3 object to be used as the ephemeris.\"\n        }\n      ]\n    },\n    \"tleData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TLEDataList\"\n        },\n        {\n          \"description\": \"The data for a TLE ephemeris, supplied directly in the request rather than through an S3 object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tle-ephemeris-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: TLEEphemeris
---
