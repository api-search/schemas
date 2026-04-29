---
description: LookupEventsResponse schema
layout: schema
name: LookupEventsResponse
properties_list:
- description: ''
  name: Events
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-lookup-events-response-schema.json
slug: cloudtrail-lookup-events-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-lookup-events-response-schema.json\",\n  \"title\": \"LookupEventsResponse\",\n  \"description\": \"LookupEventsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"EventId\": {\n            \"type\": \"string\"\n          },\n          \"EventName\": {\n            \"type\": \"string\"\n          },\n          \"EventTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"EventSource\": {\n            \"type\": \"string\"\n          },\n          \"Username\": {\n            \"type\": \"string\"\n          },\n          \"CloudTrailEvent\": {\n            \"type\": \"string\"\n         \
  \ },\n          \"ReadOnly\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-lookup-events-response-schema.json
tags:
- AWS
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: LookupEventsResponse
---
