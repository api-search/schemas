---
description: ResolveComponentCandidatesRequest schema
layout: schema
name: ResolveComponentCandidatesRequest
properties_list:
- description: ''
  name: platform
  type: object
- description: ''
  name: componentCandidates
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-resolve-component-candidates-request-schema.json
slug: iot-greengrass-resolve-component-candidates-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolve-component-candidates-request-schema.json\",\n  \"title\": \"ResolveComponentCandidatesRequest\",\n  \"description\": \"ResolveComponentCandidatesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPlatform\"\n        },\n        {\n          \"description\": \"The platform to use to resolve compatible components.\"\n        }\n      ]\n    },\n    \"componentCandidates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentCandidateList\"\n        },\n        {\n          \"description\": \"The list of components to resolve.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolve-component-candidates-request-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ResolveComponentCandidatesRequest
---
