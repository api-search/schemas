---
description: ''
layout: schema
name: DescribeFHIRDatastoreRequest
properties_list:
- description: ''
  name: DatastoreId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-datastore-request-schema.json
slug: healthlake-describe-fhir-datastore-request
source_filename: healthlake-describe-fhir-datastore-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-datastore-request-schema.json\",\n  \"title\": \"DescribeFHIRDatastoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated data store ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-datastore-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRDatastoreRequest
---
