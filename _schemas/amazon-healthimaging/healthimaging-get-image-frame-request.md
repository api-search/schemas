---
description: ''
layout: schema
name: GetImageFrameRequest
properties_list:
- description: ''
  name: imageFrameInformation
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-get-image-frame-request-schema.json
slug: healthimaging-get-image-frame-request
source_filename: healthimaging-get-image-frame-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-frame-request-schema.json\",\n  \"title\": \"GetImageFrameRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageFrameInformation\"\n  ],\n  \"properties\": {\n    \"imageFrameInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageFrameInformation\"\n        },\n        {\n          \"description\": \"Information about the image frame (pixel data) identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-frame-request-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: GetImageFrameRequest
---
