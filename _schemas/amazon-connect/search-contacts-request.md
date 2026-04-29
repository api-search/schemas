---
description: SearchContactsRequest schema from Amazon Connect Service API
layout: schema
name: SearchContactsRequest
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: InstanceId
  type: string
- description: ''
  name: TimeRange
  type: object
- description: ''
  name: SearchCriteria
  type: object
- description: The maximum number of results to return.
  name: MaxResults
  type: integer
- description: ''
  name: NextToken
  type: string
- description: ''
  name: Sort
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/search-contacts-request-schema.json
slug: search-contacts-request
source_filename: search-contacts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/search-contacts-request-schema.json\",\n  \"title\": \"SearchContactsRequest\",\n  \"description\": \"SearchContactsRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"TimeRange\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"EndTime\",\n        \"StartTime\",\n        \"Type\"\n      ],\n      \"properties\": {\n        \"Type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"INITIATION_TIMESTAMP\",\n            \"SCHEDULED_TIMESTAMP\",\n            \"CONNECTED_TO_AGENT_TIMESTAMP\",\n            \"DISCONNECT_TIMESTAMP\"\
  \n          ],\n          \"example\": \"INITIATION_TIMESTAMP\"\n        },\n        \"StartTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2025-03-15T00:00:00Z\"\n        },\n        \"EndTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2025-03-15T23:59:59Z\"\n        }\n      }\n    },\n    \"SearchCriteria\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AgentIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"QueueIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"Channels\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"The maximum number of results to return.\",\n      \"example\": 50\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"Sort\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FieldName\": {\n          \"type\": \"string\"\n        },\n        \"Order\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ASCENDING\",\n            \"DESCENDING\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"InstanceId\",\n    \"TimeRange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/search-contacts-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: SearchContactsRequest
---
