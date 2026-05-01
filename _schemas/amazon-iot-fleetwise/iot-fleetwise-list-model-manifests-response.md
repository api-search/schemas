---
description: ListModelManifestsResponse schema
layout: schema
name: ListModelManifestsResponse
properties_list:
- description: ''
  name: summaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-model-manifests-response-schema.json
slug: iot-fleetwise-list-model-manifests-response
source_filename: iot-fleetwise-list-model-manifests-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-model-manifests-response-schema.json\",\n  \"title\": \"ListModelManifestsResponse\",\n  \"description\": \"ListModelManifestsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/modelManifestSummaries\"\n        },\n        {\n          \"description\": \" A list of information about vehicle models.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-model-manifests-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListModelManifestsResponse
---
