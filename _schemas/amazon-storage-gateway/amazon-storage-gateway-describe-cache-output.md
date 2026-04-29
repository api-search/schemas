---
description: DescribeCacheOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeCacheOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DiskIds
  type: object
- description: ''
  name: CacheAllocatedInBytes
  type: object
- description: ''
  name: CacheUsedPercentage
  type: object
- description: ''
  name: CacheDirtyPercentage
  type: object
- description: ''
  name: CacheHitPercentage
  type: object
- description: ''
  name: CacheMissPercentage
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-cache-output-schema.json
slug: amazon-storage-gateway-describe-cache-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cache-output-schema.json\",\n  \"title\": \"DescribeCacheOutput\",\n  \"description\": \"DescribeCacheOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DiskIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskIds\"\n        },\n        {\n          \"description\": \"An array of strings that identify disks that are to be configured as working storage. Each string has a minimum length of 1 and maximum length of 300. You can get the disk IDs from the <a>ListLocalDisks</a> API.\"\n        }\n      ]\n    },\n    \"CacheAllocatedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\
  \n        },\n        {\n          \"description\": \"The amount of cache in bytes allocated to a gateway.\"\n        }\n      ]\n    },\n    \"CacheUsedPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"Percent use of the gateway's cache storage. This metric applies only to the gateway-cached volume setup. The sample is taken at the end of the reporting period.\"\n        }\n      ]\n    },\n    \"CacheDirtyPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The file share's contribution to the overall percentage of the gateway's cache that has not been persisted to Amazon Web Services. The sample is taken at the end of the reporting period.\"\n        }\n      ]\n    },\n    \"CacheHitPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n\
  \        },\n        {\n          \"description\": \"Percent of application read operations from the file shares that are served from cache. The sample is taken at the end of the reporting period.\"\n        }\n      ]\n    },\n    \"CacheMissPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"Percent of application read operations from the file shares that are not served from cache. The sample is taken at the end of the reporting period.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cache-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeCacheOutput
---
