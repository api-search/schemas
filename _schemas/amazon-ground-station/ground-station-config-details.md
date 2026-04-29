---
description: Details for certain <code>Config</code> object types in a contact.
layout: schema
name: ConfigDetails
properties_list:
- description: ''
  name: antennaDemodDecodeDetails
  type: object
- description: ''
  name: endpointDetails
  type: object
- description: ''
  name: s3RecordingDetails
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-config-details-schema.json
slug: ground-station-config-details
source_filename: ground-station-config-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-config-details-schema.json\",\n  \"title\": \"ConfigDetails\",\n  \"description\": \"Details for certain <code>Config</code> object types in a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"antennaDemodDecodeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AntennaDemodDecodeDetails\"\n        },\n        {\n          \"description\": \"Details for antenna demod decode <code>Config</code> in a contact.\"\n        }\n      ]\n    },\n    \"endpointDetails\": {\n      \"$ref\": \"#/components/schemas/EndpointDetails\"\n    },\n    \"s3RecordingDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3RecordingDetails\"\n        },\n        {\n          \"description\": \"Details for an S3 recording\
  \ <code>Config</code> in a contact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-config-details-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ConfigDetails
---
