---
description: List of summaries of data stores.
layout: schema
name: DatastoreSummary
properties_list:
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: datastoreName
  type: object
- description: ''
  name: datastoreStatus
  type: object
- description: ''
  name: datastoreArn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-datastore-summary-schema.json
slug: healthimaging-datastore-summary
source_filename: healthimaging-datastore-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-datastore-summary-schema.json\",\n  \"title\": \"DatastoreSummary\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"datastoreName\",\n    \"datastoreStatus\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"datastoreName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreName\"\n        },\n        {\n          \"description\": \"The data store name.\"\n        }\n      ]\n    },\n    \"datastoreStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n    \
  \    {\n          \"description\": \"The data store status.\"\n        }\n      ]\n    },\n    \"datastoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the data store.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the data store was created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the data store was last updated.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"List of summaries of data stores.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-datastore-summary-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DatastoreSummary
---
