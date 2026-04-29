---
description: ''
layout: schema
name: UpdateImageSetMetadataRequest
properties_list:
- description: ''
  name: updateImageSetMetadataUpdates
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-update-image-set-metadata-request-schema.json
slug: healthimaging-update-image-set-metadata-request
source_filename: healthimaging-update-image-set-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-update-image-set-metadata-request-schema.json\",\n  \"title\": \"UpdateImageSetMetadataRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"updateImageSetMetadataUpdates\"\n  ],\n  \"properties\": {\n    \"updateImageSetMetadataUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataUpdates\"\n        },\n        {\n          \"description\": \"Update image set metadata updates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-update-image-set-metadata-request-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: UpdateImageSetMetadataRequest
---
