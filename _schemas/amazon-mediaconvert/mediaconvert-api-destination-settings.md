---
description: Settings associated with the destination. Will vary based on the type of destination
layout: schema
name: DestinationSettings
properties_list:
- description: ''
  name: S3Settings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-destination-settings-schema.json
slug: mediaconvert-api-destination-settings
source_filename: mediaconvert-api-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-destination-settings-schema.json\",\n  \"title\": \"DestinationSettings\",\n  \"description\": \"Settings associated with the destination. Will vary based on the type of destination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Settings\"\n          },\n          \"description\": \"Settings associated with S3 destination\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-destination-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DestinationSettings
---
