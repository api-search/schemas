---
description: Copy image set information.
layout: schema
name: CopyImageSetInformation
properties_list:
- description: ''
  name: sourceImageSet
  type: object
- description: ''
  name: destinationImageSet
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-image-set-information-schema.json
slug: healthimaging-copy-image-set-information
source_filename: healthimaging-copy-image-set-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-information-schema.json\",\n  \"title\": \"CopyImageSetInformation\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sourceImageSet\"\n  ],\n  \"properties\": {\n    \"sourceImageSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CopySourceImageSetInformation\"\n        },\n        {\n          \"description\": \"The source image set.\"\n        }\n      ]\n    },\n    \"destinationImageSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CopyDestinationImageSet\"\n        },\n        {\n          \"description\": \"The destination image set.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Copy image set information.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-information-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopyImageSetInformation
---
