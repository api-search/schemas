---
description: <p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>DeleteBandwidthRateLimitInput$BandwidthType</a> </p> </li> </ul>
layout: schema
name: DeleteBandwidthRateLimitInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: BandwidthType
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-input-schema.json
slug: amazon-storage-gateway-delete-bandwidth-rate-limit-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-input-schema.json\",\n  \"title\": \"DeleteBandwidthRateLimitInput\",\n  \"description\": \"<p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>DeleteBandwidthRateLimitInput$BandwidthType</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"BandwidthType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthType\"\n        },\n        {\n          \"description\": \"<p>One of the BandwidthType values that indicates the gateway bandwidth rate limit to delete.</p> <p>Valid Values: <code>UPLOAD</code> | <code>DOWNLOAD</code> | <code>ALL</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"GatewayARN\",\n    \"BandwidthType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteBandwidthRateLimitInput
---
