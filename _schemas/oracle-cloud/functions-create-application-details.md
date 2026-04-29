---
description: CreateApplicationDetails schema from oracle-cloud-functions-openapi.yaml
layout: schema
name: CreateApplicationDetails
properties_list:
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
  name: config
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/functions-create-application-details-schema.json
slug: functions-create-application-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-create-application-details-schema.json\",\n  \"title\": \"CreateApplicationDetails\",\n  \"description\": \"CreateApplicationDetails schema from oracle-cloud-functions-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"displayName\",\n    \"subnetIds\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"subnetIds\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n   \
  \   },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/functions-create-application-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateApplicationDetails
---
