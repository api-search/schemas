---
description: ''
layout: schema
name: GetImageFrameResponse
properties_list:
- description: ''
  name: imageFrameBlob
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-get-image-frame-response-schema.json
slug: healthimaging-get-image-frame-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-frame-response-schema.json\",\n  \"title\": \"GetImageFrameResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageFrameBlob\"\n  ],\n  \"properties\": {\n    \"imageFrameBlob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PayloadBlob\"\n        },\n        {\n          \"description\": \"The blob containing the aggregated image frame information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-frame-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: GetImageFrameResponse
---
