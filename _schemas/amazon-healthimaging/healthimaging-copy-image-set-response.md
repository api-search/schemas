---
description: ''
layout: schema
name: CopyImageSetResponse
properties_list:
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: sourceImageSetProperties
  type: object
- description: ''
  name: destinationImageSetProperties
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-copy-image-set-response-schema.json
slug: healthimaging-copy-image-set-response
source_filename: healthimaging-copy-image-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-response-schema.json\",\n  \"title\": \"CopyImageSetResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"sourceImageSetProperties\",\n    \"destinationImageSetProperties\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"sourceImageSetProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CopySourceImageSetProperties\"\n        },\n        {\n          \"description\": \"The properties of the source image set.\"\n        }\n      ]\n    },\n    \"destinationImageSetProperties\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/CopyDestinationImageSetProperties\"\n        },\n        {\n          \"description\": \"The properties of the destination image set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-copy-image-set-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CopyImageSetResponse
---
