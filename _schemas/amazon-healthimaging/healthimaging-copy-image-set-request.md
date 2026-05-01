---
description: ''
layout: schema
name: CopyImageSetRequest
properties_list:
- description: ''
  name: copyImageSetInformation
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-image-set-request-schema.json
slug: healthimaging-copy-image-set-request
source_filename: healthimaging-copy-image-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-request-schema.json\",\n  \"title\": \"CopyImageSetRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"copyImageSetInformation\"\n  ],\n  \"properties\": {\n    \"copyImageSetInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CopyImageSetInformation\"\n        },\n        {\n          \"description\": \"Copy image set information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-request-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopyImageSetRequest
---
