---
description: The number of entities that are affected by one or more events. Returned by the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEntityAggregates.html">DescribeEntityAggregates</a> operation.
layout: schema
name: EntityAggregate
properties_list:
- description: ''
  name: eventArn
  type: object
- description: ''
  name: count
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-entity-aggregate-schema.json
slug: health-entity-aggregate
source_filename: health-entity-aggregate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-entity-aggregate-schema.json\",\n  \"title\": \"EntityAggregate\",\n  \"description\": \"The number of entities that are affected by one or more events. Returned by the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEntityAggregates.html\\\">DescribeEntityAggregates</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i> </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/count\"\n        },\n        {\n          \"description\": \"The number of entities that match the criteria for the specified events.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-entity-aggregate-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EntityAggregate
---
