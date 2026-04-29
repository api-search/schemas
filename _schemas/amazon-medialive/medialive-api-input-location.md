---
description: Input Location
layout: schema
name: InputLocation
properties_list:
- description: ''
  name: PasswordParam
  type: object
- description: ''
  name: Uri
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-location-schema.json
slug: medialive-api-input-location
source_filename: medialive-api-input-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-location-schema.json\",\n  \"title\": \"InputLocation\",\n  \"description\": \"Input Location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordParam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passwordParam\"\n          },\n          \"description\": \"key used to extract the password from EC2 Parameter store\"\n        }\n      ]\n    },\n    \"Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax2048\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uri\"\n          },\n          \"description\": \"Uniform Resource Identifier - This should be a path to a file accessible to the Live system\
  \ (eg. a http:// URI) depending on the output type. For example, a RTMP destination should have a uri simliar to: \\\"rtmp://fmsserver/live\\\".\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-location-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputLocation
---
