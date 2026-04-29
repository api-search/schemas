---
description: ''
layout: schema
name: DescribeFHIRDatastoreResponse
properties_list:
- description: ''
  name: DatastoreProperties
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-datastore-response-schema.json
slug: healthlake-describe-fhir-datastore-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-datastore-response-schema.json\",\n  \"title\": \"DescribeFHIRDatastoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreProperties\"\n  ],\n  \"properties\": {\n    \"DatastoreProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreProperties\"\n        },\n        {\n          \"description\": \"All properties associated with a data store, including the data store ID, data store ARN, data store name, data store status, when the data store was created, data store type version, and the data store's endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-datastore-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRDatastoreResponse
---
