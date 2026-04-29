---
description: CreateFunctionDetails schema from oracle-cloud-functions-openapi.yaml
layout: schema
name: CreateFunctionDetails
properties_list:
- description: ''
  name: applicationId
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
  name: config
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/functions-create-function-details-schema.json
slug: functions-create-function-details
source_filename: functions-create-function-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-create-function-details-schema.json\",\n  \"title\": \"CreateFunctionDetails\",\n  \"description\": \"CreateFunctionDetails schema from oracle-cloud-functions-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"applicationId\",\n    \"displayName\",\n    \"image\",\n    \"memoryInMBs\"\n  ],\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.image.oc1.iad.abcdefg123456\"\n    },\n    \"memoryInMBs\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"timeoutInSeconds\": {\n      \"type\": \"integer\",\n\
  \      \"example\": 30,\n      \"default\": 30\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-create-function-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateFunctionDetails
---
