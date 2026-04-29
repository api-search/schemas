---
description: Placeholder documentation for DescribeInputDeviceThumbnailResponse
layout: schema
name: DescribeInputDeviceThumbnailResponse
properties_list:
- description: ''
  name: Body
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-describe-input-device-thumbnail-response-schema.json
slug: medialive-api-describe-input-device-thumbnail-response
source_filename: medialive-api-describe-input-device-thumbnail-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-input-device-thumbnail-response-schema.json\",\n  \"title\": \"DescribeInputDeviceThumbnailResponse\",\n  \"description\": \"Placeholder documentation for DescribeInputDeviceThumbnailResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceThumbnail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"body\"\n          },\n          \"description\": \"The binary data for the thumbnail that the Link device has most recently sent to MediaLive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-input-device-thumbnail-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeInputDeviceThumbnailResponse
---
