---
description: The values to use to filter results from the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventTypes.html">DescribeEventTypes</a> operation.
layout: schema
name: EventTypeFilter
properties_list:
- description: ''
  name: eventTypeCodes
  type: object
- description: ''
  name: services
  type: object
- description: ''
  name: eventTypeCategories
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-type-filter-schema.json
slug: health-event-type-filter
source_filename: health-event-type-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-type-filter-schema.json\",\n  \"title\": \"EventTypeFilter\",\n  \"description\": \"The values to use to filter results from the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventTypes.html\\\">DescribeEventTypes</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypeCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventTypeCodeList\"\n        },\n        {\n          \"description\": \"A list of event type codes.\"\n        }\n      ]\n    },\n    \"services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/serviceList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services services associated with the event. For example, <code>EC2</code>,\
  \ <code>RDS</code>.\"\n        }\n      ]\n    },\n    \"eventTypeCategories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventTypeCategoryList\"\n        },\n        {\n          \"description\": \"A list of event type category codes. Possible values are <code>issue</code>, <code>accountNotification</code>, or <code>scheduledChange</code>. Currently, the <code>investigation</code> value isn't supported at this time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-type-filter-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventTypeFilter
---
