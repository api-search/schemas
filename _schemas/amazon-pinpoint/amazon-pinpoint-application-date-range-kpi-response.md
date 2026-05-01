---
description: Provides the results of a query that retrieved the data for a standard metric that applies to an application, and provides information about that query.
layout: schema
name: ApplicationDateRangeKpiResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: KpiName
  type: object
- description: ''
  name: KpiResult
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-application-date-range-kpi-response-schema.json
slug: amazon-pinpoint-application-date-range-kpi-response
source_filename: amazon-pinpoint-application-date-range-kpi-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-date-range-kpi-response-schema.json\",\n  \"title\": \"ApplicationDateRangeKpiResponse\",\n  \"description\": \"Provides the results of a query that retrieved the data for a standard metric that applies to an application, and provides information about that query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the metric applies to.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The last date and time of the date range\
  \ that was used to filter the query results, in extended ISO 8601 format. The date range is inclusive.\"\n        }\n      ]\n    },\n    \"KpiName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the metric, also referred to as a <i>key performance indicator (KPI)</i>, that the data was retrieved for. This value describes the associated metric and consists of two or more terms, which are comprised of lowercase alphanumeric characters, separated by a hyphen. For a list of possible values, see the <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/developerguide/analytics-standard-metrics.html\\\">Amazon Pinpoint Developer Guide</a>.\"\n        }\n      ]\n    },\n    \"KpiResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseKpiResult\"\n        },\n        {\n          \"description\": \"An array of objects that contains the results of the\
  \ query. Each object contains the value for the metric and metadata about that value.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null for the Application Metrics resource because the resource returns all results in a single page.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The first date and time of the date range that was used to filter the query results, in extended ISO 8601 format. The date range is inclusive.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KpiResult\",\n    \"KpiName\",\n    \"EndTime\",\n    \"StartTime\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-date-range-kpi-response-schema.json
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
title: ApplicationDateRangeKpiResponse
---
