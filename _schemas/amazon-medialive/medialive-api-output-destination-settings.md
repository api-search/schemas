---
description: Placeholder documentation for OutputDestinationSettings
layout: schema
name: OutputDestinationSettings
properties_list:
- description: ''
  name: PasswordParam
  type: object
- description: ''
  name: StreamName
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-destination-settings-schema.json
slug: medialive-api-output-destination-settings
source_filename: medialive-api-output-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-destination-settings-schema.json\",\n  \"title\": \"OutputDestinationSettings\",\n  \"description\": \"Placeholder documentation for OutputDestinationSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordParam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passwordParam\"\n          },\n          \"description\": \"key used to extract the password from EC2 Parameter store\"\n        }\n      ]\n    },\n    \"StreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamName\"\n          },\n          \"description\": \"Stream name for RTMP\
  \ destinations (URLs of type rtmp://)\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"A URL specifying a destination\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"username for destination\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputDestinationSettings
---
