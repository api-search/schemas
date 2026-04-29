---
description: Object that determines whether tracking should be used during a contact executed with this <code>Config</code> in the mission profile.
layout: schema
name: TrackingConfig
properties_list:
- description: ''
  name: autotrack
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-tracking-config-schema.json
slug: ground-station-tracking-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tracking-config-schema.json\",\n  \"title\": \"TrackingConfig\",\n  \"description\": \"Object that determines whether tracking should be used during a contact executed with this <code>Config</code> in the mission profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autotrack\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Criticality\"\n        },\n        {\n          \"description\": \"Current setting for autotrack.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"autotrack\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tracking-config-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: TrackingConfig
---
