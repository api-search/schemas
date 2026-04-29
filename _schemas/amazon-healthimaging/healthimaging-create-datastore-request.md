---
description: ''
layout: schema
name: CreateDatastoreRequest
properties_list:
- description: ''
  name: datastoreName
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: kmsKeyArn
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-create-datastore-request-schema.json
slug: healthimaging-create-datastore-request
source_filename: healthimaging-create-datastore-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-create-datastore-request-schema.json\",\n  \"title\": \"CreateDatastoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"clientToken\"\n  ],\n  \"properties\": {\n    \"datastoreName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreName\"\n        },\n        {\n          \"description\": \"The data store name.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique identifier for API idempotency.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags\
  \ provided when creating a data store.\"\n        }\n      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) assigned to the AWS Key Management Service (AWS KMS) key for accessing encrypted data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-create-datastore-request-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: CreateDatastoreRequest
---
