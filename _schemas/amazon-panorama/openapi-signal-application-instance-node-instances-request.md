---
description: SignalApplicationInstanceNodeInstancesRequest schema from Amazon Panorama
layout: schema
name: SignalApplicationInstanceNodeInstancesRequest
properties_list:
- description: ''
  name: NodeSignals
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-signal-application-instance-node-instances-request-schema.json
slug: openapi-signal-application-instance-node-instances-request
source_filename: openapi-signal-application-instance-node-instances-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-signal-application-instance-node-instances-request-schema.json\",\n  \"title\": \"SignalApplicationInstanceNodeInstancesRequest\",\n  \"description\": \"SignalApplicationInstanceNodeInstancesRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NodeSignals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeSignalList\"\n        },\n        {\n          \"description\": \"A list of signals.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NodeSignals\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-signal-application-instance-node-instances-request-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: SignalApplicationInstanceNodeInstancesRequest
---
