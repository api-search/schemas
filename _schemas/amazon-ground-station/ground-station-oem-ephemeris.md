---
description: Ephemeris data in Orbit Ephemeris Message (OEM) format.
layout: schema
name: OEMEphemeris
properties_list:
- description: ''
  name: oemData
  type: object
- description: ''
  name: s3Object
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-oem-ephemeris-schema.json
slug: ground-station-oem-ephemeris
source_filename: ground-station-oem-ephemeris-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-oem-ephemeris-schema.json\",\n  \"title\": \"OEMEphemeris\",\n  \"description\": \"Ephemeris data in Orbit Ephemeris Message (OEM) format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"oemData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnboundedString\"\n        },\n        {\n          \"description\": \"The data for an OEM ephemeris, supplied directly in the request rather than through an S3 object.\"\n        }\n      ]\n    },\n    \"s3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"Identifies the S3 object to be used as the ephemeris.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-oem-ephemeris-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: OEMEphemeris
---
