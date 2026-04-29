---
description: The detailed description of the event. Included in the information returned by the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetails.html">DescribeEventDetails</a> operation.
layout: schema
name: EventDescription
properties_list:
- description: ''
  name: latestDescription
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-description-schema.json
slug: health-event-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-description-schema.json\",\n  \"title\": \"EventDescription\",\n  \"description\": \"The detailed description of the event. Included in the information returned by the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetails.html\\\">DescribeEventDetails</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventDescription\"\n        },\n        {\n          \"description\": \"The most recent description of the event.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-description-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventDescription
---
