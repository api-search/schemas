---
description: LookupEventsRequest schema
layout: schema
name: LookupEventsRequest
properties_list:
- description: ''
  name: LookupAttributes
  type: array
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: MaxResults
  type: integer
- description: ''
  name: NextToken
  type: string
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-lookup-events-request-schema.json
slug: cloudtrail-lookup-events-request
source_filename: cloudtrail-lookup-events-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-lookup-events-request-schema.json\",\n  \"title\": \"LookupEventsRequest\",\n  \"description\": \"LookupEventsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LookupAttributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"AttributeKey\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EventId\",\n              \"EventName\",\n              \"ReadOnly\",\n              \"Username\",\n              \"ResourceType\",\n              \"ResourceName\",\n              \"EventSource\",\n              \"AccessKeyId\"\n            ]\n          },\n          \"AttributeValue\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"StartTime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-lookup-events-request-schema.json
tags:
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: LookupEventsRequest
---
