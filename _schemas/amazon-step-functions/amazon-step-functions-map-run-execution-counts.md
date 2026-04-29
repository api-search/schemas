---
description: Contains details about all of the child workflow executions started by a Map Run.
layout: schema
name: MapRunExecutionCounts
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
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-map-run-execution-counts-schema.json
slug: amazon-step-functions-map-run-execution-counts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-execution-counts-schema.json\",\n  \"title\": \"MapRunExecutionCounts\",\n  \"description\": \"Contains details about all of the child workflow executions started by a Map Run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run, but haven't started executing yet. \"\n        }\n      ]\n    },\n    \"running\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run and\
  \ are currently in-progress.\"\n        }\n      ]\n    },\n    \"succeeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run and have completed successfully.\"\n        }\n      ]\n    },\n    \"failed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run, but have failed.\"\n        }\n      ]\n    },\n    \"timedOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run and have timed out.\"\n        }\n      ]\n    },\n    \"aborted\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run and were running, but were either stopped by the user or by Step Functions because the Map Run failed. \"\n        }\n      ]\n    },\n    \"total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"The total number of child workflow executions that were started by a Map Run.\"\n        }\n      ]\n    },\n    \"resultsWritten\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedLong\"\n        },\n        {\n          \"description\": \"Returns the count of child workflow executions whose results were written by <code>ResultWriter</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/input-output-resultwriter.html\\\">ResultWriter</a>\
  \ in the <i>Step Functions Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pending\",\n    \"running\",\n    \"succeeded\",\n    \"failed\",\n    \"timedOut\",\n    \"aborted\",\n    \"total\",\n    \"resultsWritten\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-execution-counts-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: MapRunExecutionCounts
---
