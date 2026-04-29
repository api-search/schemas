---
description: A Functions application containing one or more functions.
layout: schema
name: Application
properties_list:
- description: The OCID of the application.
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: subnetIds
  type: array
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: config
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/functions-application-schema.json
slug: functions-application
source_filename: functions-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"A Functions application containing one or more functions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the application.\",\n      \"example\": \"ocid1.fnapp.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-app\"\n    },\n    \"subnetIds\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"\
  ['CREATING', 'ACTIVE', 'DELETING', 'DELETED', 'FAILED']\",\n      \"example\": \"CREATING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-application-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Application
---
