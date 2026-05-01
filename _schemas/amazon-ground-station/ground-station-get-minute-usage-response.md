---
description: <p/>
layout: schema
name: GetMinuteUsageResponse
properties_list:
- description: ''
  name: estimatedMinutesRemaining
  type: object
- description: ''
  name: isReservedMinutesCustomer
  type: object
- description: ''
  name: totalReservedMinuteAllocation
  type: object
- description: ''
  name: totalScheduledMinutes
  type: object
- description: ''
  name: upcomingMinutesScheduled
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-get-minute-usage-response-schema.json
slug: ground-station-get-minute-usage-response
source_filename: ground-station-get-minute-usage-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-minute-usage-response-schema.json\",\n  \"title\": \"GetMinuteUsageResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimatedMinutesRemaining\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Estimated number of minutes remaining for an account, specific to the month being requested.\"\n        }\n      ]\n    },\n    \"isReservedMinutesCustomer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Returns whether or not an account has signed up for the reserved minutes pricing plan, specific to the month being requested.\"\n        }\n      ]\n    },\n\
  \    \"totalReservedMinuteAllocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Total number of reserved minutes allocated, specific to the month being requested.\"\n        }\n      ]\n    },\n    \"totalScheduledMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Total scheduled minutes for an account, specific to the month being requested.\"\n        }\n      ]\n    },\n    \"upcomingMinutesScheduled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Upcoming minutes scheduled for an account, specific to the month being requested.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-minute-usage-response-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: GetMinuteUsageResponse
---
