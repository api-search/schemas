---
description: ResolveComponentCandidatesResponse schema
layout: schema
name: ResolveComponentCandidatesResponse
properties_list:
- description: ''
  name: resolvedComponentVersions
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-resolve-component-candidates-response-schema.json
slug: iot-greengrass-resolve-component-candidates-response
source_filename: iot-greengrass-resolve-component-candidates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolve-component-candidates-response-schema.json\",\n  \"title\": \"ResolveComponentCandidatesResponse\",\n  \"description\": \"ResolveComponentCandidatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resolvedComponentVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolvedComponentVersionsList\"\n        },\n        {\n          \"description\": \"A list of components that meet the requirements that you specify in the request. This list includes each component's recipe that you can use to install the component.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolve-component-candidates-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ResolveComponentCandidatesResponse
---
