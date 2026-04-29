---
description: ''
layout: schema
name: DeleteFHIRDatastoreResponse
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
schema_file: json-schema/healthlake-delete-fhir-datastore-response-schema.json
slug: healthlake-delete-fhir-datastore-response
source_filename: healthlake-delete-fhir-datastore-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-delete-fhir-datastore-response-schema.json\",\n  \"title\": \"DeleteFHIRDatastoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\",\n    \"DatastoreArn\",\n    \"DatastoreStatus\",\n    \"DatastoreEndpoint\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated ID for the data store to be deleted.\"\n        }\n      ]\n    },\n    \"DatastoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that gives AWS HealthLake access permission.\"\n        }\n      ]\n    },\n    \"DatastoreStatus\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n        {\n          \"description\": \"The status of the data store that the user has requested to be deleted. \"\n        }\n      ]\n    },\n    \"DatastoreEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoundedLengthString\"\n        },\n        {\n          \"description\": \"The AWS endpoint for the data store the user has requested to be deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-delete-fhir-datastore-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DeleteFHIRDatastoreResponse
---
