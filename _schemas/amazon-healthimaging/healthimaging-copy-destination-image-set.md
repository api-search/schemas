---
description: Copy the destination image set.
layout: schema
name: CopyDestinationImageSet
properties_list:
- description: ''
  name: imageSetId
  type: object
- description: ''
  name: latestVersionId
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-destination-image-set-schema.json
slug: healthimaging-copy-destination-image-set
source_filename: healthimaging-copy-destination-image-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-destination-image-set-schema.json\",\n  \"title\": \"CopyDestinationImageSet\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetId\",\n    \"latestVersionId\"\n  ],\n  \"properties\": {\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier for the destination image set.\"\n        }\n      ]\n    },\n    \"latestVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetExternalVersionId\"\n        },\n        {\n          \"description\": \"The latest version identifier for the destination image set.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Copy the destination image set.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-destination-image-set-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopyDestinationImageSet
---
