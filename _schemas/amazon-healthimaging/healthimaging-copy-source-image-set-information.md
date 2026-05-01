---
description: Copy source image set information.
layout: schema
name: CopySourceImageSetInformation
properties_list:
- description: ''
  name: latestVersionId
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-source-image-set-information-schema.json
slug: healthimaging-copy-source-image-set-information
source_filename: healthimaging-copy-source-image-set-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-source-image-set-information-schema.json\",\n  \"title\": \"CopySourceImageSetInformation\",\n  \"type\": \"object\",\n  \"required\": [\n    \"latestVersionId\"\n  ],\n  \"properties\": {\n    \"latestVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetExternalVersionId\"\n        },\n        {\n          \"description\": \"The latest version identifier for the source image set.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Copy source image set information.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-source-image-set-information-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopySourceImageSetInformation
---
