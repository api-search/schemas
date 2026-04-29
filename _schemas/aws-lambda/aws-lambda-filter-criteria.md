---
description: An object that contains the filters for an event source. Event filtering enables you to control which records from an event source Lambda sends to your function.
layout: schema
name: FilterCriteria
properties_list:
- description: A list of filters
  name: Filters
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-filter-criteria-schema.json
slug: aws-lambda-filter-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterCriteria\",\n  \"type\": \"object\",\n  \"description\": \"An object that contains the filters for an event source. Event filtering enables you to control which records from an event source Lambda sends to your function.\",\n  \"properties\": {\n    \"Filters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of filters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-filter-criteria-schema.json
tags: []
title: FilterCriteria
---
