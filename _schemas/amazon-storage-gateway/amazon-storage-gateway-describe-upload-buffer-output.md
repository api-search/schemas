---
description: DescribeUploadBufferOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeUploadBufferOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DiskIds
  type: object
- description: ''
  name: UploadBufferUsedInBytes
  type: object
- description: ''
  name: UploadBufferAllocatedInBytes
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-upload-buffer-output-schema.json
slug: amazon-storage-gateway-describe-upload-buffer-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-upload-buffer-output-schema.json\",\n  \"title\": \"DescribeUploadBufferOutput\",\n  \"description\": \"DescribeUploadBufferOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DiskIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskIds\"\n        },\n        {\n          \"description\": \"An array of the gateway's local disk IDs that are configured as working storage. Each local disk ID is specified as a string (minimum length of 1 and maximum length of 300). If no local disks are configured as working storage, then the DiskIds array is empty.\"\n        }\n      ]\n    },\n    \"UploadBufferUsedInBytes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The total number of bytes being used in the gateway's upload buffer.\"\n        }\n      ]\n    },\n    \"UploadBufferAllocatedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The total number of bytes allocated in the gateway's as upload buffer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-upload-buffer-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeUploadBufferOutput
---
