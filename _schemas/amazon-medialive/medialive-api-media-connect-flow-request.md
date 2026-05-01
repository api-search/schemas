---
description: The settings for a MediaConnect Flow.
layout: schema
name: MediaConnectFlowRequest
properties_list:
- description: ''
  name: FlowArn
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-media-connect-flow-request-schema.json
slug: medialive-api-media-connect-flow-request
source_filename: medialive-api-media-connect-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-media-connect-flow-request-schema.json\",\n  \"title\": \"MediaConnectFlowRequest\",\n  \"description\": \"The settings for a MediaConnect Flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the MediaConnect Flow that you want to use as a source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-media-connect-flow-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MediaConnectFlowRequest
---
