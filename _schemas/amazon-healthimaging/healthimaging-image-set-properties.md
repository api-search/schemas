---
description: The image set properties.
layout: schema
name: ImageSetProperties
properties_list:
- description: ''
  name: imageSetId
  type: object
- description: ''
  name: versionId
  type: object
- description: ''
  name: imageSetState
  type: object
- description: ''
  name: ImageSetWorkflowStatus
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: deletedAt
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-image-set-properties-schema.json
slug: healthimaging-image-set-properties
source_filename: healthimaging-image-set-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-set-properties-schema.json\",\n  \"title\": \"ImageSetProperties\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetId\",\n    \"versionId\",\n    \"imageSetState\"\n  ],\n  \"properties\": {\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier.\"\n        }\n      ]\n    },\n    \"versionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetExternalVersionId\"\n        },\n        {\n          \"description\": \"The image set version identifier.\"\n        }\n      ]\n    },\n    \"imageSetState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetState\"\n    \
  \    },\n        {\n          \"description\": \"The image set state.\"\n        }\n      ]\n    },\n    \"ImageSetWorkflowStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetWorkflowStatus\"\n        },\n        {\n          \"description\": \"The image set workflow status.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the image set properties were created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the image set properties were updated.\"\n        }\n      ]\n    },\n    \"deletedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The\
  \ timestamp when the image set properties were deleted.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The error message thrown if an image set action fails.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The image set properties.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-image-set-properties-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ImageSetProperties
---
