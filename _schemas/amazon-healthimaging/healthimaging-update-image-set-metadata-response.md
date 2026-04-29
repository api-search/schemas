---
description: ''
layout: schema
name: UpdateImageSetMetadataResponse
properties_list:
- description: ''
  name: datastoreId
  type: object
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
  name: message
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-update-image-set-metadata-response-schema.json
slug: healthimaging-update-image-set-metadata-response
source_filename: healthimaging-update-image-set-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-update-image-set-metadata-response-schema.json\",\n  \"title\": \"UpdateImageSetMetadataResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"imageSetId\",\n    \"latestVersionId\",\n    \"imageSetState\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier.\"\n        }\n      ]\n    },\n    \"latestVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetExternalVersionId\"\
  \n        },\n        {\n          \"description\": \"The latest image set version identifier.\"\n        }\n      ]\n    },\n    \"imageSetState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetState\"\n        },\n        {\n          \"description\": \"The image set state.\"\n        }\n      ]\n    },\n    \"imageSetWorkflowStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetWorkflowStatus\"\n        },\n        {\n          \"description\": \"The image set workflow status.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when image set metadata was created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp\
  \ when image set metadata was updated.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The error message thrown if an update image set metadata action fails.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-update-image-set-metadata-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: UpdateImageSetMetadataResponse
---
