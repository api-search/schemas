---
description: DescribeEventDetailsResponse schema from Amazon Health Dashboard API
layout: schema
name: DescribeEventDetailsResponse
properties_list:
- description: ''
  name: successfulSet
  type: object
- description: ''
  name: failedSet
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-event-details-response-schema.json
slug: health-describe-event-details-response
source_filename: health-describe-event-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-response-schema.json\",\n  \"title\": \"DescribeEventDetailsResponse\",\n  \"description\": \"DescribeEventDetailsResponse schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"successfulSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribeEventDetailsSuccessfulSet\"\n        },\n        {\n          \"description\": \"Information about the events that could be retrieved.\"\n        }\n      ]\n    },\n    \"failedSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribeEventDetailsFailedSet\"\n        },\n        {\n          \"description\": \"Error messages for any events that could not be retrieved.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-details-response-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEventDetailsResponse
---
