---
description: Describes a bandwidth rate limit interval for a gateway. A bandwidth rate limit schedule consists of one or more bandwidth rate limit intervals. A bandwidth rate limit interval defines a period of time on one or more days of the week, during which bandwidth rate limits are specified for uploading, downloading, or both.
layout: schema
name: BandwidthRateLimitInterval
properties_list:
- description: ''
  name: StartHourOfDay
  type: object
- description: ''
  name: StartMinuteOfHour
  type: object
- description: ''
  name: EndHourOfDay
  type: object
- description: ''
  name: EndMinuteOfHour
  type: object
- description: ''
  name: DaysOfWeek
  type: object
- description: ''
  name: AverageUploadRateLimitInBitsPerSec
  type: object
- description: ''
  name: AverageDownloadRateLimitInBitsPerSec
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-bandwidth-rate-limit-interval-schema.json
slug: amazon-storage-gateway-bandwidth-rate-limit-interval
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-bandwidth-rate-limit-interval-schema.json\",\n  \"title\": \"BandwidthRateLimitInterval\",\n  \"description\": \" Describes a bandwidth rate limit interval for a gateway. A bandwidth rate limit schedule consists of one or more bandwidth rate limit intervals. A bandwidth rate limit interval defines a period of time on one or more days of the week, during which bandwidth rate limits are specified for uploading, downloading, or both. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartHourOfDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\n        },\n        {\n          \"description\": \" The hour of the day to start the bandwidth rate limit interval. \"\n        }\n      ]\n    },\n    \"StartMinuteOfHour\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinuteOfHour\"\n        },\n        {\n          \"description\": \" The minute of the hour to start the bandwidth rate limit interval. The interval begins at the start of that minute. To begin an interval exactly at the start of the hour, use the value <code>0</code>. \"\n        }\n      ]\n    },\n    \"EndHourOfDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\n        },\n        {\n          \"description\": \" The hour of the day to end the bandwidth rate limit interval. \"\n        }\n      ]\n    },\n    \"EndMinuteOfHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinuteOfHour\"\n        },\n        {\n          \"description\": \"<p> The minute of the hour to end the bandwidth rate limit interval. </p> <important> <p> The bandwidth rate limit interval ends at the end of the minute. To end an interval at the end of an hour,\
  \ use the value <code>59</code>. </p> </important>\"\n        }\n      ]\n    },\n    \"DaysOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DaysOfWeek\"\n        },\n        {\n          \"description\": \" The days of the week component of the bandwidth rate limit interval, represented as ordinal numbers from 0 to 6, where 0 represents Sunday and 6 represents Saturday. \"\n        }\n      ]\n    },\n    \"AverageUploadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthUploadRateLimit\"\n        },\n        {\n          \"description\": \" The average upload rate limit component of the bandwidth rate limit interval, in bits per second. This field does not appear in the response if the upload rate limit is not set. \"\n        }\n      ]\n    },\n    \"AverageDownloadRateLimitInBitsPerSec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthDownloadRateLimit\"\
  \n        },\n        {\n          \"description\": \" The average download rate limit component of the bandwidth rate limit interval, in bits per second. This field does not appear in the response if the download rate limit is not set. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StartHourOfDay\",\n    \"StartMinuteOfHour\",\n    \"EndHourOfDay\",\n    \"EndMinuteOfHour\",\n    \"DaysOfWeek\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-bandwidth-rate-limit-interval-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: BandwidthRateLimitInterval
---
