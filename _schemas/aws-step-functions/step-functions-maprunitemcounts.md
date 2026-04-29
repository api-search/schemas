---
description: Contains details about items that were processed in all of the child workflow executions that were started by a Map Run.
layout: schema
name: MapRunItemCounts
properties_list:
- description: ''
  name: pending
  type: object
- description: ''
  name: running
  type: object
- description: ''
  name: succeeded
  type: object
- description: ''
  name: failed
  type: object
- description: ''
  name: timedOut
  type: object
- description: ''
  name: aborted
  type: object
- description: ''
  name: total
  type: object
- description: ''
  name: resultsWritten
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-maprunitemcounts-schema.json
slug: step-functions-maprunitemcounts
source_filename: step-functions-maprunitemcounts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MapRunItemCounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pending\": {},\n    \"running\": {},\n    \"succeeded\": {},\n    \"failed\": {},\n    \"timedOut\": {},\n    \"aborted\": {},\n    \"total\": {},\n    \"resultsWritten\": {}\n  },\n  \"required\": [\n    \"pending\",\n    \"running\",\n    \"succeeded\",\n    \"failed\",\n    \"timedOut\",\n    \"aborted\",\n    \"total\",\n    \"resultsWritten\"\n  ],\n  \"description\": \"Contains details about items that were processed in all of the child workflow executions that were started by a Map Run.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-maprunitemcounts-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: MapRunItemCounts
---
