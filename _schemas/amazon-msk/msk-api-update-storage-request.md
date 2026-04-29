---
description: <p>Request object for UpdateStorage api. Its used to update the storage attributes for the cluster.</p>
layout: schema
name: UpdateStorageRequest
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: ProvisionedThroughput
  type: object
- description: ''
  name: StorageMode
  type: object
- description: ''
  name: VolumeSizeGB
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-storage-request-schema.json
slug: msk-api-update-storage-request
source_filename: msk-api-update-storage-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-storage-request-schema.json\",\n  \"title\": \"UpdateStorageRequest\",\n  \"description\": \"\\n            <p>Request object for UpdateStorage api. Its used to update the storage attributes for the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The version of cluster to update from. A successful operation will then generate a new version.</p>\"\n        }\n      ]\n    },\n    \"ProvisionedThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n        },\n   \
  \     {\n          \"xml\": {\n            \"name\": \"provisionedThroughput\"\n          },\n          \"description\": \"\\n            <p>EBS volume provisioned throughput information.</p>\"\n        }\n      ]\n    },\n    \"StorageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageMode\"\n          },\n          \"description\": \"\\n            <p>Controls storage mode for supported storage tiers.</p>\"\n        }\n      ]\n    },\n    \"VolumeSizeGB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeSizeGB\"\n          },\n          \"description\": \"\\n            <p>size of the EBS volume to update.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-storage-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateStorageRequest
---
