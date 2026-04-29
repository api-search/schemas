---
description: Dataflow details for the destination side.
layout: schema
name: Destination
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
  name: dataflowDestinationRegion
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-destination-schema.json
slug: ground-station-destination
source_filename: ground-station-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-destination-schema.json\",\n  \"title\": \"Destination\",\n  \"description\": \"Dataflow details for the destination side.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigDetails\"\n        },\n        {\n          \"description\": \"Additional details for a <code>Config</code>, if type is dataflow endpoint or antenna demod decode.\"\n        }\n      ]\n    },\n    \"configId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"configType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigCapabilityType\"\
  \n        },\n        {\n          \"description\": \"Type of a <code>Config</code>.\"\n        }\n      ]\n    },\n    \"dataflowDestinationRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Region of a dataflow destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-destination-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: Destination
---
