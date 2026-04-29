---
description: ''
layout: schema
name: CreateFHIRDatastoreResponse
properties_list:
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: DatastoreArn
  type: object
- description: ''
  name: DatastoreStatus
  type: object
- description: ''
  name: DatastoreEndpoint
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-create-fhir-datastore-response-schema.json
slug: healthlake-create-fhir-datastore-response
source_filename: healthlake-create-fhir-datastore-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-create-fhir-datastore-response-schema.json\",\n  \"title\": \"CreateFHIRDatastoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\",\n    \"DatastoreArn\",\n    \"DatastoreStatus\",\n    \"DatastoreEndpoint\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated data store id. This id is in the output from the initial data store creation call.\"\n        }\n      ]\n    },\n    \"DatastoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreArn\"\n        },\n        {\n          \"description\": \"The data store ARN is generated during the creation of the data store and\
  \ can be found in the output from the initial data store creation call.\"\n        }\n      ]\n    },\n    \"DatastoreStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n        {\n          \"description\": \"The status of the FHIR data store.\"\n        }\n      ]\n    },\n    \"DatastoreEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoundedLengthString\"\n        },\n        {\n          \"description\": \"The AWS endpoint for the created data store.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-create-fhir-datastore-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: CreateFHIRDatastoreResponse
---
