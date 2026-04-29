---
description: A request to claim an AWS Elemental device that you have purchased from a third-party vendor.
layout: schema
name: ClaimDeviceRequest
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-claim-device-request-schema.json
slug: medialive-api-claim-device-request
source_filename: medialive-api-claim-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-claim-device-request-schema.json\",\n  \"title\": \"ClaimDeviceRequest\",\n  \"description\": \"A request to claim an AWS Elemental device that you have purchased from a third-party vendor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The id of the device you want to claim.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-claim-device-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClaimDeviceRequest
---
