---
description: ''
layout: schema
name: DeleteDatastoreResponse
properties_list:
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: datastoreStatus
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-delete-datastore-response-schema.json
slug: healthimaging-delete-datastore-response
source_filename: healthimaging-delete-datastore-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-delete-datastore-response-schema.json\",\n  \"title\": \"DeleteDatastoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"datastoreStatus\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"datastoreStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n        {\n          \"description\": \"The data store status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-delete-datastore-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DeleteDatastoreResponse
---
