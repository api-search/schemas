---
description: Reference to an OutputDestination ID defined in the channel
layout: schema
name: OutputLocationRef
properties_list:
- description: ''
  name: DestinationRefId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-location-ref-schema.json
slug: medialive-api-output-location-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-location-ref-schema.json\",\n  \"title\": \"OutputLocationRef\",\n  \"description\": \"Reference to an OutputDestination ID defined in the channel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationRefId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationRefId\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-location-ref-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputLocationRef
---
