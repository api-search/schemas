---
description: DescribeEventAggregatesRequest schema from Amazon Health Dashboard API
layout: schema
name: DescribeEventAggregatesRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: ''
  name: aggregateField
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-describe-event-aggregates-request-schema.json
slug: health-describe-event-aggregates-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-aggregates-request-schema.json\",\n  \"title\": \"DescribeEventAggregatesRequest\",\n  \"description\": \"DescribeEventAggregatesRequest schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventFilter\"\n        },\n        {\n          \"description\": \"Values to narrow the results returned.\"\n        }\n      ]\n    },\n    \"aggregateField\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventAggregateField\"\n        },\n        {\n          \"description\": \"The only currently supported value is <code>eventTypeCategory</code>.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/maxResults\"\n        },\n        {\n          \"description\": \"The maximum number of items to return in one batch, between 10 and 100, inclusive.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next batch of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"aggregateField\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-describe-event-aggregates-request-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: DescribeEventAggregatesRequest
---
