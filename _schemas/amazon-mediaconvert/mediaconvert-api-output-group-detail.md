---
description: Contains details about the output groups specified in the job settings.
layout: schema
name: OutputGroupDetail
properties_list:
- description: ''
  name: OutputDetails
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-group-detail-schema.json
slug: mediaconvert-api-output-group-detail
source_filename: mediaconvert-api-output-group-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-detail-schema.json\",\n  \"title\": \"OutputGroupDetail\",\n  \"description\": \"Contains details about the output groups specified in the job settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputDetails\"\n          },\n          \"description\": \"Details about the output\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-detail-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputGroupDetail
---
