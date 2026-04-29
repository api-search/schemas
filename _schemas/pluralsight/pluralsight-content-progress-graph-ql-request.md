---
description: GraphQLRequest from Pluralsight API
layout: schema
name: GraphQLRequest
properties_list:
- description: The GraphQL query string
  name: query
  type: string
- description: Variables for the GraphQL query
  name: variables
  type: object
- description: Name of the operation to execute
  name: operationName
  type: string
provider_name: Pluralsight
provider_slug: pluralsight
schema_file: json-schema/pluralsight-content-progress-graph-ql-request-schema.json
slug: pluralsight-content-progress-graph-ql-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-content-progress-graph-ql-request-schema.json\",\n  \"title\": \"GraphQLRequest\",\n  \"description\": \"GraphQLRequest from Pluralsight API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL query string\",\n      \"example\": \"example_value\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Variables for the GraphQL query\"\n    },\n    \"operationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the operation to execute\",\n      \"example\": \"Example Course\"\n    }\n  },\n  \"required\": [\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-content-progress-graph-ql-request-schema.json
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
title: GraphQLRequest
---
