---
description: ''
layout: schema
name: GetImageSetMetadataResponse
properties_list:
- description: ''
  name: imageSetMetadataBlob
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-get-image-set-metadata-response-schema.json
slug: healthimaging-get-image-set-metadata-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-set-metadata-response-schema.json\",\n  \"title\": \"GetImageSetMetadataResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetMetadataBlob\"\n  ],\n  \"properties\": {\n    \"imageSetMetadataBlob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetMetadataBlob\"\n        },\n        {\n          \"description\": \"The blob containing the aggregated metadata information for the image set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-image-set-metadata-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: GetImageSetMetadataResponse
---
