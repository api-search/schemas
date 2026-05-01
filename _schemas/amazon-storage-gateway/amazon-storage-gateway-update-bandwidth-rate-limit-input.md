---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateBandwidthRateLimitInput$AverageDownloadRateLimitInBitsPerSec</a> </p> </li> <li> <p> <a>UpdateBandwidthRateLimitInput$AverageUploadRateLimitInBitsPerSec</a> </p> </li> </ul>
layout: schema
name: UpdateBandwidthRateLimitInput
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
schema_file: json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-input-schema.json
slug: amazon-storage-gateway-update-bandwidth-rate-limit-input
source_filename: amazon-storage-gateway-update-bandwidth-rate-limit-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-input-schema.json\",\n  \"title\": \"UpdateBandwidthRateLimitInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateBandwidthRateLimitInput$AverageDownloadRateLimitInBitsPerSec</a> </p> </li> <li> <p> <a>UpdateBandwidthRateLimitInput$AverageUploadRateLimitInBitsPerSec</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"AverageUploadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthUploadRateLimit\"\n        },\n        {\n          \"description\": \"The average upload bandwidth rate limit in bits per second.\"\n\
  \        }\n      ]\n    },\n    \"AverageDownloadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthDownloadRateLimit\"\n        },\n        {\n          \"description\": \"The average download bandwidth rate limit in bits per second.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateBandwidthRateLimitInput
---
