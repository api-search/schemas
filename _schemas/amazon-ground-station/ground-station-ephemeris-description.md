---
description: Description of ephemeris.
layout: schema
name: EphemerisDescription
properties_list:
- description: ''
  name: ephemerisData
  type: object
- description: ''
  name: sourceS3Object
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ephemeris-description-schema.json
slug: ground-station-ephemeris-description
source_filename: ground-station-ephemeris-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-description-schema.json\",\n  \"title\": \"EphemerisDescription\",\n  \"description\": \"Description of ephemeris.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ephemerisData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnboundedString\"\n        },\n        {\n          \"description\": \"Supplied ephemeris data.\"\n        }\n      ]\n    },\n    \"sourceS3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"Source S3 object used for the ephemeris.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-description-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EphemerisDescription
---
