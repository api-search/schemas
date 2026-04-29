---
description: ListFlywheelsRequest schema
layout: schema
name: ListFlywheelsRequest
properties_list:
- description: ''
  name: Filter
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-flywheels-request-schema.json
slug: openapi.yml-list-flywheels-request
source_filename: openapi.yml-list-flywheels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheels-request-schema.json\",\n  \"title\": \"ListFlywheelsRequest\",\n  \"description\": \"ListFlywheelsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelFilter\"\n        },\n        {\n          \"description\": \"Filters the flywheels that are returned. You can filter flywheels on their status, or the date and time that they were submitted. You can only set one filter at a time. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsInteger\"\n        },\n        {\n          \"description\": \"Maximum number of results to return in a response. The default is 100.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheels-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListFlywheelsRequest
---
