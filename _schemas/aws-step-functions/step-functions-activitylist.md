---
description: ''
layout: schema
name: ActivityList
properties_list: []
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-activitylist-schema.json
slug: step-functions-activitylist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"activityArn\": {},\n      \"name\": {},\n      \"creationDate\": {}\n    },\n    \"required\": [\n      \"activityArn\",\n      \"name\",\n      \"creationDate\"\n    ],\n    \"description\": \"Contains details about an activity.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-activitylist-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: ActivityList
---
