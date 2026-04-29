---
description: UpdateEphemerisRequest schema from Amazon Ground Station API
layout: schema
name: UpdateEphemerisRequest
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: priority
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-update-ephemeris-request-schema.json
slug: ground-station-update-ephemeris-request
source_filename: ground-station-update-ephemeris-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-ephemeris-request-schema.json\",\n  \"title\": \"UpdateEphemerisRequest\",\n  \"description\": \"UpdateEphemerisRequest schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the ephemeris is enabled or not. Changing this value will not require the ephemeris to be re-validated.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"A name string associated with the ephemeris. Used as a human-readable identifier for the ephemeris.\"\n        }\n      ]\n\
  \    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisPriority\"\n        },\n        {\n          \"description\": \"<p>Customer-provided priority score to establish the order in which overlapping ephemerides should be used.</p> <p>The default for customer-provided ephemeris priority is 1, and higher numbers take precedence.</p> <p>Priority must be 1 or greater</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-ephemeris-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: UpdateEphemerisRequest
---
