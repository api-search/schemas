---
description: GraphQLResponse from Pluralsight API
layout: schema
name: GraphQLResponse
properties_list:
- description: The query result data
  name: data
  type: object
- description: Any errors that occurred during query execution
  name: errors
  type: array
provider_name: Pluralsight
provider_slug: pluralsight
schema_file: json-schema/pluralsight-course-progress-graph-ql-response-schema.json
slug: pluralsight-course-progress-graph-ql-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-course-progress-graph-ql-response-schema.json\",\n  \"title\": \"GraphQLResponse\",\n  \"description\": \"GraphQLResponse from Pluralsight API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The query result data\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GraphQLError\"\n      },\n      \"description\": \"Any errors that occurred during query execution\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-course-progress-graph-ql-response-schema.json
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
title: GraphQLResponse
---
