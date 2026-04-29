---
description: ''
layout: schema
name: DeleteImageSetResponse
properties_list:
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: imageSetId
  type: object
- description: ''
  name: imageSetState
  type: object
- description: ''
  name: imageSetWorkflowStatus
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-delete-image-set-response-schema.json
slug: healthimaging-delete-image-set-response
source_filename: healthimaging-delete-image-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-delete-image-set-response-schema.json\",\n  \"title\": \"DeleteImageSetResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"imageSetId\",\n    \"imageSetState\",\n    \"imageSetWorkflowStatus\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"imageSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetId\"\n        },\n        {\n          \"description\": \"The image set identifier.\"\n        }\n      ]\n    },\n    \"imageSetState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetState\"\
  \n        },\n        {\n          \"description\": \"The image set state.\"\n        }\n      ]\n    },\n    \"imageSetWorkflowStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetWorkflowStatus\"\n        },\n        {\n          \"description\": \"The image set workflow status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-delete-image-set-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DeleteImageSetResponse
---
