---
description: Multiplex output destination settings
layout: schema
name: MultiplexOutputDestination
properties_list:
- description: ''
  name: MediaConnectSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-output-destination-schema.json
slug: medialive-api-multiplex-output-destination
source_filename: medialive-api-multiplex-output-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-output-destination-schema.json\",\n  \"title\": \"MultiplexOutputDestination\",\n  \"description\": \"Multiplex output destination settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MediaConnectSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexMediaConnectOutputDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaConnectSettings\"\n          },\n          \"description\": \"Multiplex MediaConnect output destination settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-output-destination-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexOutputDestination
---
