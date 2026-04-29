---
description: Multiplex MediaConnect output destination settings.
layout: schema
name: MultiplexMediaConnectOutputDestinationSettings
properties_list:
- description: ''
  name: EntitlementArn
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-media-connect-output-destination-settings-schema.json
slug: medialive-api-multiplex-media-connect-output-destination-settings
source_filename: medialive-api-multiplex-media-connect-output-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-media-connect-output-destination-settings-schema.json\",\n  \"title\": \"MultiplexMediaConnectOutputDestinationSettings\",\n  \"description\": \"Multiplex MediaConnect output destination settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementArn\"\n          },\n          \"description\": \"The MediaConnect entitlement ARN available as a Flow source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-media-connect-output-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexMediaConnectOutputDestinationSettings
---
