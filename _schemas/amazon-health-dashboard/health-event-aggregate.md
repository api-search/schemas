---
description: The number of events of each issue type. Returned by the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventAggregates.html">DescribeEventAggregates</a> operation.
layout: schema
name: EventAggregate
properties_list:
- description: ''
  name: aggregateValue
  type: object
- description: ''
  name: count
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-aggregate-schema.json
slug: health-event-aggregate
source_filename: health-event-aggregate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-aggregate-schema.json\",\n  \"title\": \"EventAggregate\",\n  \"description\": \"The number of events of each issue type. Returned by the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventAggregates.html\\\">DescribeEventAggregates</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregateValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/aggregateValue\"\n        },\n        {\n          \"description\": \"The issue type for the associated count.\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/count\"\n        },\n        {\n          \"description\": \"The number of events of the associated issue type.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-aggregate-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventAggregate
---
