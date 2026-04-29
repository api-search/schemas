---
description: GetCurrentMetricDataRequest schema from Amazon Connect Service API
layout: schema
name: GetCurrentMetricDataRequest
properties_list:
- description: The queues, up to 100, or channels, to use to filter the metrics returned.
  name: Filters
  type: object
- description: ''
  name: Groupings
  type: array
- description: ''
  name: CurrentMetrics
  type: array
- description: ''
  name: NextToken
  type: string
- description: ''
  name: MaxResults
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/get-current-metric-data-request-schema.json
slug: get-current-metric-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-current-metric-data-request-schema.json\",\n  \"title\": \"GetCurrentMetricDataRequest\",\n  \"description\": \"GetCurrentMetricDataRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"type\": \"object\",\n      \"description\": \"The queues, up to 100, or channels, to use to filter the metrics returned.\",\n      \"properties\": {\n        \"Queues\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"Channels\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"VOICE\",\n              \"CHAT\",\n              \"TASK\"\n            ]\n          }\n        }\n      }\n\
  \    },\n    \"Groupings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CurrentMetrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"AGENTS_ONLINE\",\n              \"AGENTS_AVAILABLE\",\n              \"AGENTS_ON_CALL\",\n              \"AGENTS_NON_PRODUCTIVE\",\n              \"AGENTS_AFTER_CONTACT_WORK\",\n              \"AGENTS_ERROR\",\n              \"AGENTS_STAFFED\",\n              \"CONTACTS_IN_QUEUE\",\n              \"OLDEST_CONTACT_AGE\",\n              \"CONTACTS_SCHEDULED\",\n              \"AGENTS_ON_CONTACT\",\n              \"SLOTS_ACTIVE\",\n              \"SLOTS_AVAILABLE\"\n            ]\n          },\n          \"Unit\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"SECONDS\",\n              \"COUNT\",\n       \
  \       \"PERCENT\"\n            ]\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"CurrentMetrics\",\n    \"Filters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-current-metric-data-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: GetCurrentMetricDataRequest
---
