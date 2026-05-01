---
description: An object representing the method header to be matched.
layout: schema
name: GrpcMetadataMatchMethod
properties_list:
- description: ''
  name: exact
  type: object
- description: ''
  name: prefix
  type: object
- description: 'An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, '
  name: range
  type: object
- description: ''
  name: regex
  type: object
- description: ''
  name: suffix
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-metadata-match-method-schema.json
slug: app-mesh-grpc-metadata-match-method
source_filename: app-mesh-grpc-metadata-match-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The exact method header to be matched on.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The specified beginning characters of the method header to be matched on.\"\n        }\n      ]\n    },\n    \"range\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"end\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The end of the range.\"\n            }\n          ]\n        },\n        \"start\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n          \
  \  },\n            {\n              \"description\": \"The start of the range.\"\n            }\n          ]\n        }\n      },\n      \"required\": [\n        \"end\",\n        \"start\"\n      ],\n      \"description\": \"An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.\"\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The regex used to match the method header.\"\n        }\n      ]\n    },\n    \"suffix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The specified ending characters of the method header to match on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing\
  \ the method header to be matched.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-metadata-match-method-schema.json\",\n  \"title\": \"GrpcMetadataMatchMethod\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-metadata-match-method-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcMetadataMatchMethod
---
