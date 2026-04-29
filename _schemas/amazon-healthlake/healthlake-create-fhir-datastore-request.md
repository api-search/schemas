---
description: ''
layout: schema
name: CreateFHIRDatastoreRequest
properties_list:
- description: ''
  name: DatastoreName
  type: object
- description: ''
  name: DatastoreTypeVersion
  type: object
- description: ''
  name: SseConfiguration
  type: object
- description: ''
  name: PreloadDataConfig
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: IdentityProviderConfiguration
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-create-fhir-datastore-request-schema.json
slug: healthlake-create-fhir-datastore-request
source_filename: healthlake-create-fhir-datastore-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-create-fhir-datastore-request-schema.json\",\n  \"title\": \"CreateFHIRDatastoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreTypeVersion\"\n  ],\n  \"properties\": {\n    \"DatastoreName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreName\"\n        },\n        {\n          \"description\": \"The user generated name for the data store.\"\n        }\n      ]\n    },\n    \"DatastoreTypeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FHIRVersion\"\n        },\n        {\n          \"description\": \"The FHIR version of the data store. The only supported version is R4.\"\n        }\n      ]\n    },\n    \"SseConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfiguration\"\
  \n        },\n        {\n          \"description\": \" The server-side encryption key configuration for a customer provided encryption key specified for creating a data store. \"\n        }\n      ]\n    },\n    \"PreloadDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreloadDataConfig\"\n        },\n        {\n          \"description\": \"Optional parameter to preload data upon creation of the data store. Currently, the only supported preloaded data is synthetic data generated from Synthea.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientTokenString\"\n        },\n        {\n          \"description\": \"Optional user provided token used for ensuring idempotency.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" Resource tags\
  \ that are applied to a data store when it is created. \"\n        }\n      ]\n    },\n    \"IdentityProviderConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderConfiguration\"\n        },\n        {\n          \"description\": \"The configuration of the identity provider that you want to use for your data store.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-create-fhir-datastore-request-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: CreateFHIRDatastoreRequest
---
