---
description: ''
layout: schema
name: GetDatastoreResponse
properties_list:
- description: ''
  name: datastoreProperties
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-get-datastore-response-schema.json
slug: healthimaging-get-datastore-response
source_filename: healthimaging-get-datastore-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-datastore-response-schema.json\",\n  \"title\": \"GetDatastoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreProperties\"\n  ],\n  \"properties\": {\n    \"datastoreProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreProperties\"\n        },\n        {\n          \"description\": \"The data store properties.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-get-datastore-response-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: GetDatastoreResponse
---
