---
description: A serverless function.
layout: schema
name: Function
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: applicationId
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: image
  type: string
- description: ''
  name: memoryInMBs
  type: integer
- description: ''
  name: timeoutInSeconds
  type: integer
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: invokeEndpoint
  type: string
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: config
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/functions-function-schema.json
slug: functions-function
source_filename: functions-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-function-schema.json\",\n  \"title\": \"Function\",\n  \"description\": \"A serverless function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-function\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"example\": \"iad.ocir.io/my-namespace/my-app/my-function:0.0.1\"\n    },\n    \"memoryInMBs\": {\n      \"type\": \"integer\",\n      \"example\"\
  : 256\n    },\n    \"timeoutInSeconds\": {\n      \"type\": \"integer\",\n      \"example\": 30\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['CREATING', 'ACTIVE', 'INACTIVE', 'UPDATING', 'DELETING', 'DELETED', 'FAILED']\",\n      \"example\": \"CREATING\"\n    },\n    \"invokeEndpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-function-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Function
---
