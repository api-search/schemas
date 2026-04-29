---
description: Aggregate status of Agent components.
layout: schema
name: AggregateStatus
properties_list:
- description: ''
  name: signatureMap
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-aggregate-status-schema.json
slug: ground-station-aggregate-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-aggregate-status-schema.json\",\n  \"title\": \"AggregateStatus\",\n  \"description\": \"Aggregate status of Agent components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"signatureMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignatureMap\"\n        },\n        {\n          \"description\": \"Sparse map of failure signatures.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentStatus\"\n        },\n        {\n          \"description\": \"Aggregate status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-aggregate-status-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AggregateStatus
---
