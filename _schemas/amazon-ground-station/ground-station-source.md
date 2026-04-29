---
description: Dataflow details for the source side.
layout: schema
name: Source
properties_list:
- description: ''
  name: configDetails
  type: object
- description: ''
  name: configId
  type: object
- description: ''
  name: configType
  type: object
- description: ''
  name: dataflowSourceRegion
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-source-schema.json
slug: ground-station-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"Dataflow details for the source side.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigDetails\"\n        },\n        {\n          \"description\": \"Additional details for a <code>Config</code>, if type is <code>dataflow-endpoint</code> or <code>antenna-downlink-demod-decode</code> \"\n        }\n      ]\n    },\n    \"configId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"UUID of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"configType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigCapabilityType\"\
  \n        },\n        {\n          \"description\": \"Type of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"dataflowSourceRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Region of a dataflow source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-source-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: Source
---
