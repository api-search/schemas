---
description: DescribeBandwidthRateLimitScheduleOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeBandwidthRateLimitScheduleOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: BandwidthRateLimitIntervals
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-schedule-output-schema.json
slug: amazon-storage-gateway-describe-bandwidth-rate-limit-schedule-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-schedule-output-schema.json\",\n  \"title\": \"DescribeBandwidthRateLimitScheduleOutput\",\n  \"description\": \"DescribeBandwidthRateLimitScheduleOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"BandwidthRateLimitIntervals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthRateLimitIntervals\"\n        },\n        {\n          \"description\": \" An array that contains the bandwidth rate limit intervals for a tape or volume gateway. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-bandwidth-rate-limit-schedule-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeBandwidthRateLimitScheduleOutput
---
