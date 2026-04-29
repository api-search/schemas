---
description: Information about the image frame (pixel data) identifier.
layout: schema
name: ImageFrameInformation
properties_list:
- description: ''
  name: imageFrameId
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-image-frame-information-schema.json
slug: healthimaging-image-frame-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-frame-information-schema.json\",\n  \"title\": \"ImageFrameInformation\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageFrameId\"\n  ],\n  \"properties\": {\n    \"imageFrameId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageFrameId\"\n        },\n        {\n          \"description\": \"The image frame (pixel data) identifier.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about the image frame (pixel data) identifier.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-frame-information-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ImageFrameInformation
---
