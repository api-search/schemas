---
description: GraphQLError from Pluralsight API
layout: schema
name: GraphQLError
properties_list:
- description: Error message
  name: message
  type: string
- description: ''
  name: locations
  type: array
- description: ''
  name: path
  type: array
provider_name: Pluralsight
provider_slug: pluralsight
schema_file: json-schema/pluralsight-skills-assessment-graph-ql-error-schema.json
slug: pluralsight-skills-assessment-graph-ql-error
source_filename: pluralsight-skills-assessment-graph-ql-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-skills-assessment-graph-ql-error-schema.json\",\n  \"title\": \"GraphQLError\",\n  \"description\": \"GraphQLError from Pluralsight API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"example_value\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"line\": {\n            \"type\": \"integer\"\n          },\n          \"column\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"path\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/json-schema/pluralsight-skills-assessment-graph-ql-error-schema.json
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
title: GraphQLError
---
