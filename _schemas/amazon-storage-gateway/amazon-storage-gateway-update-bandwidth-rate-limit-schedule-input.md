---
description: UpdateBandwidthRateLimitScheduleInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateBandwidthRateLimitScheduleInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: BandwidthRateLimitIntervals
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-schedule-input-schema.json
slug: amazon-storage-gateway-update-bandwidth-rate-limit-schedule-input
source_filename: amazon-storage-gateway-update-bandwidth-rate-limit-schedule-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-schedule-input-schema.json\",\n  \"title\": \"UpdateBandwidthRateLimitScheduleInput\",\n  \"description\": \"UpdateBandwidthRateLimitScheduleInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"BandwidthRateLimitIntervals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthRateLimitIntervals\"\n        },\n        {\n          \"description\": \" An array containing bandwidth rate limit schedule intervals for a gateway. When no bandwidth rate limit intervals have been scheduled, the array is empty. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"\
  BandwidthRateLimitIntervals\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-bandwidth-rate-limit-schedule-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateBandwidthRateLimitScheduleInput
---
