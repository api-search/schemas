---
description: Summary of the image set metadata.
layout: schema
name: ImageSetsMetadataSummary
properties_list:
- description: ''
  name: imageSetId
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: DICOMTags
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-image-sets-metadata-summary-schema.json
slug: healthimaging-image-sets-metadata-summary
source_filename: healthimaging-image-sets-metadata-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-sets-metadata-summary-schema.json\",\n  \"title\": \"ImageSetsMetadataSummary\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetId\"\n  ],\n  \"properties\": {\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The image set version.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time an image set is created\
  \ in AWS HealthImaging. Sample creation date is provided in <code>1985-04-12T23:20:50.52Z</code> format.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when an image was last updated in AWS HealthImaging.\"\n        }\n      ]\n    },\n    \"DICOMTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DICOMTags\"\n        },\n        {\n          \"description\": \"The DICOM tags associated with the image set.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Summary of the image set metadata.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-sets-metadata-summary-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ImageSetsMetadataSummary
---
