---
description: 'A JSON object containing the following fields:'
layout: schema
name: DescribeWorkingStorageOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DiskIds
  type: object
- description: ''
  name: WorkingStorageUsedInBytes
  type: object
- description: ''
  name: WorkingStorageAllocatedInBytes
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-working-storage-output-schema.json
slug: amazon-storage-gateway-describe-working-storage-output
source_filename: amazon-storage-gateway-describe-working-storage-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-working-storage-output-schema.json\",\n  \"title\": \"DescribeWorkingStorageOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DiskIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskIds\"\n        },\n        {\n          \"description\": \"An array of the gateway's local disk IDs that are configured as working storage. Each local disk ID is specified as a string (minimum length of 1 and maximum length of 300). If no local disks are configured as working storage, then the DiskIds array is empty.\"\n        }\n      ]\n    },\n    \"WorkingStorageUsedInBytes\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The total working storage in bytes in use by the gateway. If no working storage is configured for the gateway, this field returns 0.\"\n        }\n      ]\n    },\n    \"WorkingStorageAllocatedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The total working storage in bytes allocated for the gateway. If no working storage is configured for the gateway, this field returns 0.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-working-storage-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeWorkingStorageOutput
---
