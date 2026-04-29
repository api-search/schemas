---
description: Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey activity, and provides information about that query.
layout: schema
name: JourneyExecutionActivityMetricsResponse
properties_list:
- description: ''
  name: ActivityType
  type: object
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: JourneyActivityId
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
schema_file: json-schema/amazon-pinpoint-journey-execution-activity-metrics-response-schema.json
slug: amazon-pinpoint-journey-execution-activity-metrics-response
source_filename: amazon-pinpoint-journey-execution-activity-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-execution-activity-metrics-response-schema.json\",\n  \"title\": \"JourneyExecutionActivityMetricsResponse\",\n  \"description\": \"Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey activity, and provides information about that query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActivityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The type of activity that the metric applies to. Possible values are:</p> <ul><li><p>CONDITIONAL_SPLIT - For a yes/no split activity, which is an activity that sends participants down one of two paths in a journey.</p></li> <li><p>HOLDOUT - For a holdout activity, which is\
  \ an activity that stops a journey for a specified percentage of participants.</p></li> <li><p>MESSAGE - For an email activity, which is an activity that sends an email message to participants.</p></li> <li><p>MULTI_CONDITIONAL_SPLIT - For a multivariate split activity, which is an activity that sends participants down one of as many as five paths in a journey.</p></li> <li><p>RANDOM_SPLIT - For a random split activity, which is an activity that sends specified percentages of participants down one of as many as five paths in a journey.</p></li> <li><p>WAIT - For a wait activity, which is an activity that waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.</p></li></ul>\"\n        }\n      ]\n    },\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the\
  \ metric applies to.\"\n        }\n      ]\n    },\n    \"JourneyActivityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the activity that the metric applies to.\"\n        }\n      ]\n    },\n    \"JourneyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the journey that the metric applies to.\"\n        }\n      ]\n    },\n    \"LastEvaluatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when Amazon Pinpoint last evaluated the execution status of the activity and updated the data for the metric.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\
  \n        },\n        {\n          \"description\": \"A JSON object that contains the results of the query. The results vary depending on the type of activity (ActivityType). For information about the structure and contents of the results, see the <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/developerguide/analytics-standard-metrics.html\\\">Amazon Pinpoint Developer Guide</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Metrics\",\n    \"JourneyId\",\n    \"LastEvaluatedTime\",\n    \"JourneyActivityId\",\n    \"ActivityType\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-execution-activity-metrics-response-schema.json
tags:
- AWS
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
title: JourneyExecutionActivityMetricsResponse
---
