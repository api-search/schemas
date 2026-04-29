---
description: A paginated collection of problems.
layout: schema
name: ProblemCollection
properties_list:
- description: Cursor for the next page of results. Null if no more pages.
  name: nextPageKey
  type: string
- description: The total number of problems matching the query.
  name: totalCount
  type: integer
- description: The number of results returned on this page.
  name: pageSize
  type: integer
- description: The list of problems on this page.
  name: problems
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-api-v2-problem-collection-schema.json
slug: problems-api-v2-problem-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-collection-schema.json\",\n  \"title\": \"ProblemCollection\",\n  \"description\": \"A paginated collection of problems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results. Null if no more pages.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of problems matching the query.\",\n      \"example\": 500\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned on this page.\",\n      \"example\": 500\n    },\n    \"problems\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"The list of problems on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Problem\"\n      },\n      \"example\": [\n        {\n          \"problemId\": \"abc123\",\n          \"displayId\": \"abc123\",\n          \"title\": \"example-value\",\n          \"severityLevel\": \"AVAILABILITY\",\n          \"status\": \"OPEN\",\n          \"startTime\": 1718153645993,\n          \"endTime\": 1718153645993,\n          \"affectedEntities\": [\n            {\n              \"entityId\": \"abc123\",\n              \"name\": \"Production Service\",\n              \"type\": \"STANDARD\"\n            }\n          ],\n          \"impactedEntities\": [\n            {\n              \"entityId\": \"abc123\",\n              \"name\": \"Production Service\",\n              \"type\": \"STANDARD\"\n            }\n          ],\n          \"rootCauseEntity\": \"example-value\",\n          \"managementZones\": [\n            {\n              \"id\": \"abc123\",\n              \"\
  name\": \"Production Service\"\n            }\n          ],\n          \"problemFilters\": [\n            {\n              \"id\": \"abc123\",\n              \"name\": \"Production Service\"\n            }\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-collection-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: ProblemCollection
---
