---
description: Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey, and provides information about that query.
layout: schema
name: JourneyExecutionMetricsResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: JourneyId
  type: object
- description: ''
  name: LastEvaluatedTime
  type: object
- description: ''
  name: Metrics
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-execution-metrics-response-schema.json
slug: amazon-pinpoint-journey-execution-metrics-response
source_filename: amazon-pinpoint-journey-execution-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-execution-metrics-response-schema.json\",\n  \"title\": \"JourneyExecutionMetricsResponse\",\n  \"description\": \"Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey, and provides information about that query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the metric applies to.\"\n        }\n      ]\n    },\n    \"JourneyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the journey that\
  \ the metric applies to.\"\n        }\n      ]\n    },\n    \"LastEvaluatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when Amazon Pinpoint last evaluated the journey and updated the data for the metric.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A JSON object that contains the results of the query. For information about the structure and contents of the results, see the <a href=\\\"https://docs.aws.amazon.com//pinpoint/latest/developerguide/analytics-standard-metrics.html\\\">Amazon Pinpoint Developer Guide</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Metrics\",\n    \"JourneyId\",\n    \"LastEvaluatedTime\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-execution-metrics-response-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: JourneyExecutionMetricsResponse
---
