---
description: 'A JSON object containing the following fields:'
layout: schema
name: DescribeBandwidthRateLimitOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: AverageUploadRateLimitInBitsPerSec
  type: object
- description: ''
  name: AverageDownloadRateLimitInBitsPerSec
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-output-schema.json
slug: amazon-storage-gateway-describe-bandwidth-rate-limit-output
source_filename: amazon-storage-gateway-describe-bandwidth-rate-limit-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-output-schema.json\",\n  \"title\": \"DescribeBandwidthRateLimitOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"AverageUploadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthUploadRateLimit\"\n        },\n        {\n          \"description\": \"The average upload bandwidth rate limit in bits per second. This field does not appear in the response if the upload rate limit is not set.\"\n        }\n      ]\n    },\n    \"AverageDownloadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthDownloadRateLimit\"\
  \n        },\n        {\n          \"description\": \"The average download bandwidth rate limit in bits per second. This field does not appear in the response if the download rate limit is not set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeBandwidthRateLimitOutput
---
