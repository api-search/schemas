---
description: Placeholder documentation for DescribeScheduleResponse
layout: schema
name: DescribeScheduleResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ScheduleActions
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-describe-schedule-response-schema.json
slug: medialive-api-describe-schedule-response
source_filename: medialive-api-describe-schedule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-schedule-response-schema.json\",\n  \"title\": \"DescribeScheduleResponse\",\n  \"description\": \"Placeholder documentation for DescribeScheduleResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The next token; for use in pagination.\"\n        }\n      ]\n    },\n    \"ScheduleActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfScheduleAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scheduleActions\"\n          },\n          \"description\": \"The list of actions in\
  \ the schedule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-schedule-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeScheduleResponse
---
