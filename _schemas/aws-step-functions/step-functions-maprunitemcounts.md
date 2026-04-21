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
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: MapRunItemCounts
---
