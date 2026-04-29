---
description: Copy source image set properties.
layout: schema
name: CopySourceImageSetProperties
properties_list:
- description: ''
  name: imageSetId
  type: object
- description: ''
  name: latestVersionId
  type: object
- description: ''
  name: imageSetState
  type: object
- description: ''
  name: imageSetWorkflowStatus
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: imageSetArn
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-source-image-set-properties-schema.json
slug: healthimaging-copy-source-image-set-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-source-image-set-properties-schema.json\",\n  \"title\": \"CopySourceImageSetProperties\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetId\",\n    \"latestVersionId\"\n  ],\n  \"properties\": {\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier for the copied source image set.\"\n        }\n      ]\n    },\n    \"latestVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetExternalVersionId\"\n        },\n        {\n          \"description\": \"The latest version identifier for the copied source image set.\"\n        }\n      ]\n    },\n    \"imageSetState\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/ImageSetState\"\n        },\n        {\n          \"description\": \"The image set state of the copied source image set.\"\n        }\n      ]\n    },\n    \"imageSetWorkflowStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetWorkflowStatus\"\n        },\n        {\n          \"description\": \"The workflow status of the copied source image set.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the source image set properties were created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the source image set properties were updated.\"\n        }\n      ]\n    },\n    \"imageSetArn\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) assigned to the source image set.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Copy source image set properties.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-source-image-set-properties-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopySourceImageSetProperties
---
