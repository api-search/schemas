---
description: Details about an antenna demod decode <code>Config</code> used in a contact.
layout: schema
name: AntennaDemodDecodeDetails
properties_list:
- description: ''
  name: outputNode
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-antenna-demod-decode-details-schema.json
slug: ground-station-antenna-demod-decode-details
source_filename: ground-station-antenna-demod-decode-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-demod-decode-details-schema.json\",\n  \"title\": \"AntennaDemodDecodeDetails\",\n  \"description\": \"Details about an antenna demod decode <code>Config</code> used in a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputNode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Name of an antenna demod decode output node used in a contact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-demod-decode-details-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AntennaDemodDecodeDetails
---
