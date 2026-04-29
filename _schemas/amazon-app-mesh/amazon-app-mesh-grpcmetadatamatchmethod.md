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
- description: ''
  name: range
  type: object
- description: ''
  name: regex
  type: object
- description: ''
  name: suffix
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-grpcmetadatamatchmethod-schema.json
slug: amazon-app-mesh-grpcmetadatamatchmethod
source_filename: amazon-app-mesh-grpcmetadatamatchmethod-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GrpcMetadataMatchMethod\",\n  \"description\": \"An object representing the method header to be matched.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {},\n    \"prefix\": {},\n    \"range\": {\n      \"$ref\": \"#/definitions/MatchRange\"\n    },\n    \"regex\": {},\n    \"suffix\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-grpcmetadatamatchmethod-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GrpcMetadataMatchMethod
---
