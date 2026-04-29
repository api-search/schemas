---
description: Displays the properties of the data store, including the ID, ARN, name, and the status of the data store.
layout: schema
name: DatastoreProperties
properties_list:
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: DatastoreArn
  type: object
- description: ''
  name: DatastoreName
  type: object
- description: ''
  name: DatastoreStatus
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: DatastoreTypeVersion
  type: object
- description: ''
  name: DatastoreEndpoint
  type: object
- description: ''
  name: SseConfiguration
  type: object
- description: ''
  name: PreloadDataConfig
  type: object
- description: ''
  name: IdentityProviderConfiguration
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-datastore-properties-schema.json
slug: healthlake-datastore-properties
source_filename: healthlake-datastore-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-datastore-properties-schema.json\",\n  \"title\": \"DatastoreProperties\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\",\n    \"DatastoreArn\",\n    \"DatastoreStatus\",\n    \"DatastoreTypeVersion\",\n    \"DatastoreEndpoint\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated ID number for the data store.\"\n        }\n      ]\n    },\n    \"DatastoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name used in the creation of the data store.\"\n        }\n      ]\n    },\n    \"DatastoreName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreName\"\n        },\n        {\n          \"description\": \"The user-generated name for the data store.\"\n        }\n      ]\n    },\n    \"DatastoreStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreStatus\"\n        },\n        {\n          \"description\": \"The status of the data store.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that a data store was created. \"\n        }\n      ]\n    },\n    \"DatastoreTypeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FHIRVersion\"\n        },\n        {\n          \"description\": \"The FHIR version. Only R4 version data is supported.\"\n        }\n      ]\n    },\n    \"DatastoreEndpoint\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The AWS endpoint for the data store. Each data store will have it's own endpoint with data store ID in the endpoint URL.\"\n        }\n      ]\n    },\n    \"SseConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfiguration\"\n        },\n        {\n          \"description\": \" The server-side encryption key configuration for a customer provided encryption key (CMK). \"\n        }\n      ]\n    },\n    \"PreloadDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreloadDataConfig\"\n        },\n        {\n          \"description\": \"The preloaded data configuration for the data store. Only data preloaded from Synthea is supported.\"\n        }\n      ]\n    },\n    \"IdentityProviderConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderConfiguration\"\
  \n        },\n        {\n          \"description\": \"The identity provider that you selected when you created the data store.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Displays the properties of the data store, including the ID, ARN, name, and the status of the data store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-datastore-properties-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DatastoreProperties
---
