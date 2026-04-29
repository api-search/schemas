---
description: SignalApplicationInstanceNodeInstancesResponse schema from Amazon Panorama
layout: schema
name: SignalApplicationInstanceNodeInstancesResponse
properties_list:
- description: ''
  name: ApplicationInstanceId
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-signal-application-instance-node-instances-response-schema.json
slug: openapi-signal-application-instance-node-instances-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-signal-application-instance-node-instances-response-schema.json\",\n  \"title\": \"SignalApplicationInstanceNodeInstancesResponse\",\n  \"description\": \"SignalApplicationInstanceNodeInstancesResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"An application instance ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationInstanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-signal-application-instance-node-instances-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: SignalApplicationInstanceNodeInstancesResponse
---
