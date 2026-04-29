---
description: GetMetricDataRequest schema from Amazon Connect Service API
layout: schema
name: GetMetricDataRequest
properties_list:
- description: The timestamp, in UNIX Epoch time format, at which to start the reporting interval.
  name: StartTime
  type: string
- description: The timestamp, in UNIX Epoch time format, at which to end the reporting interval.
  name: EndTime
  type: string
- description: The queues, up to 100, or channels, to use to filter the metrics returned.
  name: Filters
  type: object
- description: ''
  name: Groupings
  type: array
- description: ''
  name: HistoricalMetrics
  type: array
- description: ''
  name: NextToken
  type: string
- description: ''
  name: MaxResults
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/get-metric-data-request-schema.json
slug: get-metric-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-metric-data-request-schema.json\",\n  \"title\": \"GetMetricDataRequest\",\n  \"description\": \"GetMetricDataRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp, in UNIX Epoch time format, at which to start the reporting interval.\",\n      \"example\": \"2025-03-15T00:00:00Z\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp, in UNIX Epoch time format, at which to end the reporting interval.\",\n      \"example\": \"2025-03-15T23:59:59Z\"\n    },\n    \"Filters\": {\n      \"type\": \"object\",\n      \"description\": \"The queues, up to 100, or channels,\
  \ to use to filter the metrics returned.\",\n      \"properties\": {\n        \"Queues\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"Channels\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"VOICE\",\n              \"CHAT\",\n              \"TASK\"\n            ]\n          }\n        }\n      }\n    },\n    \"Groupings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"QUEUE\",\n          \"CHANNEL\",\n          \"ROUTING_PROFILE\",\n          \"ROUTING_STEP_EXPRESSION\"\n        ]\n      }\n    },\n    \"HistoricalMetrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metric.\",\n\
  \            \"enum\": [\n              \"CONTACTS_QUEUED\",\n              \"CONTACTS_HANDLED\",\n              \"CONTACTS_ABANDONED\",\n              \"CONTACTS_CONSULTED\",\n              \"CONTACTS_AGENT_HUNG_UP_FIRST\",\n              \"CONTACTS_HANDLED_INCOMING\",\n              \"CONTACTS_HANDLED_OUTBOUND\",\n              \"CONTACTS_HOLD_ABANDONS\",\n              \"CONTACTS_TRANSFERRED_IN\",\n              \"CONTACTS_TRANSFERRED_OUT\",\n              \"CONTACTS_TRANSFERRED_IN_FROM_QUEUE\",\n              \"CONTACTS_TRANSFERRED_OUT_FROM_QUEUE\",\n              \"CONTACTS_MISSED\",\n              \"CALLBACK_CONTACTS_HANDLED\",\n              \"HANDLE_TIME\",\n              \"AFTER_CONTACT_WORK_TIME\",\n              \"QUEUED_TIME\",\n              \"ABANDON_TIME\",\n              \"QUEUE_ANSWER_TIME\",\n              \"HOLD_TIME\",\n              \"INTERACTION_TIME\",\n              \"INTERACTION_AND_HOLD_TIME\",\n              \"SERVICE_LEVEL\"\n            ]\n          },\n  \
  \        \"Unit\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"SECONDS\",\n              \"COUNT\",\n              \"PERCENT\"\n            ]\n          },\n          \"Statistic\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"SUM\",\n              \"MAX\",\n              \"AVG\"\n            ]\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"EndTime\",\n    \"Filters\",\n    \"HistoricalMetrics\",\n    \"StartTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-metric-data-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: GetMetricDataRequest
---
