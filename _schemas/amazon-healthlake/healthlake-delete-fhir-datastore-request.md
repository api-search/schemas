---
description: ''
layout: schema
name: DeleteFHIRDatastoreRequest
properties_list:
- description: ''
  name: DatastoreId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-delete-fhir-datastore-request-schema.json
slug: healthlake-delete-fhir-datastore-request
source_filename: healthlake-delete-fhir-datastore-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-delete-fhir-datastore-request-schema.json\",\n  \"title\": \"DeleteFHIRDatastoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \" The AWS-generated ID for the data store to be deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-delete-fhir-datastore-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DeleteFHIRDatastoreRequest
---
