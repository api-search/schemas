---
description: Endpoint settings for a PUSH type input.
layout: schema
name: InputDestinationRequest
properties_list:
- description: ''
  name: StreamName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-destination-request-schema.json
slug: medialive-api-input-destination-request
source_filename: medialive-api-input-destination-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-request-schema.json\",\n  \"title\": \"InputDestinationRequest\",\n  \"description\": \"Endpoint settings for a PUSH type input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamName\"\n          },\n          \"description\": \"A unique name for the location the RTMP stream is being pushed\\nto.\\n\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDestinationRequest
---
