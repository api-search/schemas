---
description: DescribeEntityAggregatesResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeEntityAggregatesResponse
properties_list:
- description: ''
  name: entityAggregates
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-entity-aggregates-response-schema.json
slug: health-describe-entity-aggregates-response
source_filename: health-describe-entity-aggregates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-entity-aggregates-response-schema.json\",\n  \"title\": \"DescribeEntityAggregatesResponse\",\n  \"description\": \"DescribeEntityAggregatesResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityAggregates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityAggregateList\"\n        },\n        {\n          \"description\": \"The number of entities that are affected by each of the specified events.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-entity-aggregates-response-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEntityAggregatesResponse
---
